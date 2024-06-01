# Comparing `tmp/breadslicer-0.0.1.tar.gz` & `tmp/breadslicer-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "breadslicer-0.0.1.tar", max compression
+gzip compressed data, was "breadslicer-0.0.2.tar", max compression
```

## Comparing `breadslicer-0.0.1.tar` & `breadslicer-0.0.2.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0     9858 2024-06-01 09:52:39.538888 breadslicer-0.0.1/README.md
--rw-r--r--   0        0        0     1232 2024-06-01 15:52:54.332657 breadslicer-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-06-01 09:52:39.458887 breadslicer-0.0.1/src/breadslicer/__init__.py
--rw-r--r--   0        0        0        0 2024-06-01 09:52:39.538888 breadslicer-0.0.1/src/breadslicer/application/__init__.py
--rw-r--r--   0        0        0     3019 2024-06-01 09:52:39.538888 breadslicer-0.0.1/src/breadslicer/application/app.py
--rw-r--r--   0        0        0     1950 2024-06-01 09:52:39.538888 breadslicer-0.0.1/src/breadslicer/application/renderer.py
--rw-r--r--   0        0        0     1849 2024-06-01 09:52:39.538888 breadslicer-0.0.1/src/breadslicer/application/slice.py
--rw-r--r--   0        0        0        0 2024-06-01 09:52:39.538888 breadslicer-0.0.1/src/breadslicer/components/__init__.py
--rw-r--r--   0        0        0      346 2024-06-01 09:52:39.538888 breadslicer-0.0.1/src/breadslicer/components/base.py
--rw-r--r--   0        0        0      655 2024-06-01 09:52:39.538888 breadslicer-0.0.1/src/breadslicer/components/choice.py
--rw-r--r--   0        0        0      494 2024-06-01 09:52:39.538888 breadslicer-0.0.1/src/breadslicer/components/confirm.py
--rw-r--r--   0        0        0      476 2024-06-01 09:52:39.538888 breadslicer-0.0.1/src/breadslicer/components/editor.py
--rw-r--r--   0        0        0      516 2024-06-01 09:52:39.538888 breadslicer-0.0.1/src/breadslicer/components/multiple_choice.py
--rw-r--r--   0        0        0      473 2024-06-01 09:52:39.538888 breadslicer-0.0.1/src/breadslicer/components/password.py
--rw-r--r--   0        0        0     1195 2024-06-01 09:52:39.538888 breadslicer-0.0.1/src/breadslicer/components/text.py
--rwxr-xr-x   0        0        0     1823 2024-06-01 09:52:39.538888 breadslicer-0.0.1/src/breadslicer/main.py
--rw-r--r--   0        0        0        0 2024-06-01 09:52:39.458887 breadslicer-0.0.1/src/breadslicer/py.typed
--rw-r--r--   0        0        0        0 2024-06-01 09:52:39.538888 breadslicer-0.0.1/src/breadslicer/utility/__init__.py
--rw-r--r--   0        0        0      349 2024-06-01 09:52:39.538888 breadslicer-0.0.1/src/breadslicer/utility/abstractdataclass.py
--rw-r--r--   0        0        0     1841 2024-06-01 09:52:39.538888 breadslicer-0.0.1/src/breadslicer/utility/command.py
--rw-r--r--   0        0        0      486 2024-06-01 09:52:39.538888 breadslicer-0.0.1/src/breadslicer/utility/fs.py
--rw-r--r--   0        0        0      274 2024-06-01 09:52:39.538888 breadslicer-0.0.1/src/breadslicer/utility/git.py
--rw-r--r--   0        0        0        0 2024-06-01 09:52:39.538888 breadslicer-0.0.1/src/opinionated/__init__.py
--rw-r--r--   0        0        0     2975 2024-06-01 09:52:39.538888 breadslicer-0.0.1/src/opinionated/bread.py
--rw-r--r--   0        0        0     3231 2024-06-01 09:52:39.538888 breadslicer-0.0.1/src/opinionated/cleanup.py
--rw-r--r--   0        0        0     1296 2024-06-01 09:52:39.538888 breadslicer-0.0.1/src/opinionated/dependencies.py
--rw-r--r--   0        0        0      263 2024-06-01 09:52:39.538888 breadslicer-0.0.1/src/opinionated/includes/Dockerfile.alpine
--rw-r--r--   0        0        0      334 2024-06-01 09:52:39.538888 breadslicer-0.0.1/src/opinionated/includes/Dockerfile.debian
--rw-r--r--   0        0        0     1302 2024-06-01 09:52:39.538888 breadslicer-0.0.1/src/opinionated/includes/Dockerfile.python
--rw-r--r--   0        0        0      339 2024-06-01 09:52:39.538888 breadslicer-0.0.1/src/opinionated/includes/Dockerfile.slim
--rw-r--r--   0        0        0     2905 2024-06-01 09:52:39.538888 breadslicer-0.0.1/src/opinionated/includes/app.gitlab-ci.yml
--rw-r--r--   0        0        0     1917 2024-06-01 09:52:39.538888 breadslicer-0.0.1/src/opinionated/includes/lib.gitlab-ci.yml
--rw-r--r--   0        0        0     2259 2024-06-01 09:52:39.538888 breadslicer-0.0.1/src/opinionated/includes/utils.gitlab-ci.yml
--rw-r--r--   0        0        0      124 2024-06-01 09:52:39.538888 breadslicer-0.0.1/src/opinionated/project_types.py
--rw-r--r--   0        0        0        0 2024-06-01 09:52:39.538888 breadslicer-0.0.1/src/opinionated/py.typed
--rw-r--r--   0        0        0     4512 2024-06-01 09:52:39.538888 breadslicer-0.0.1/src/opinionated/questions.py
--rw-r--r--   0        0        0     2169 2024-06-01 09:52:39.538888 breadslicer-0.0.1/src/opinionated/templates/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0       61 2024-06-01 09:52:39.538888 breadslicer-0.0.1/src/opinionated/templates/.dockerignore
--rw-r--r--   0        0        0     1298 2024-06-01 09:52:39.538888 breadslicer-0.0.1/src/opinionated/templates/.envrc
--rw-r--r--   0        0        0      121 2024-06-01 09:52:39.538888 breadslicer-0.0.1/src/opinionated/templates/.flake8
--rw-r--r--   0        0        0        0 2024-06-01 09:52:39.538888 breadslicer-0.0.1/src/opinionated/templates/.github/workflows/.keep
--rw-r--r--   0        0        0      208 2024-06-01 09:52:39.538888 breadslicer-0.0.1/src/opinionated/templates/.gitignore
--rw-r--r--   0        0        0        0 2024-06-01 09:52:39.538888 breadslicer-0.0.1/src/opinionated/templates/.gitlab/.keep
--rw-r--r--   0        0        0      146 2024-06-01 09:52:39.538888 breadslicer-0.0.1/src/opinionated/templates/.gitlab-ci.yml
--rw-r--r--   0        0        0      186 2024-06-01 09:52:39.538888 breadslicer-0.0.1/src/opinionated/templates/.pre-commit-config.yaml
--rwxr-xr-x   0        0        0     3420 2024-06-01 09:52:39.538888 breadslicer-0.0.1/src/opinionated/templates/.print_help.py
--rw-r--r--   0        0        0      685 2024-06-01 09:52:39.538888 breadslicer-0.0.1/src/opinionated/templates/.vscode/extensions.json
--rw-r--r--   0        0        0     2666 2024-06-01 09:52:39.542888 breadslicer-0.0.1/src/opinionated/templates/.vscode/launch.json
--rw-r--r--   0        0        0      643 2024-06-01 09:52:39.542888 breadslicer-0.0.1/src/opinionated/templates/.vscode/settings.json
--rw-r--r--   0        0        0     1238 2024-06-01 09:52:39.542888 breadslicer-0.0.1/src/opinionated/templates/.vscode/tasks.json
--rw-r--r--   0        0        0      211 2024-06-01 09:52:39.542888 breadslicer-0.0.1/src/opinionated/templates/Dockerfile
--rw-r--r--   0        0        0     4888 2024-06-01 09:52:39.542888 breadslicer-0.0.1/src/opinionated/templates/Makefile
--rw-r--r--   0        0        0        0 2024-06-01 09:52:39.542888 breadslicer-0.0.1/src/opinionated/templates/README.md
--rwxr-xr-x   0        0        0      674 2024-06-01 09:52:39.542888 breadslicer-0.0.1/src/opinionated/templates/django/project_template/manage.py-tpl
--rw-r--r--   0        0        0        0 2024-06-01 09:52:39.542888 breadslicer-0.0.1/src/opinionated/templates/django/project_template/project_name/__init__.py-tpl
--rw-r--r--   0        0        0      428 2024-06-01 09:52:39.542888 breadslicer-0.0.1/src/opinionated/templates/django/project_template/project_name/asgi.py-tpl
--rw-r--r--   0        0        0     3390 2024-06-01 09:52:39.542888 breadslicer-0.0.1/src/opinionated/templates/django/project_template/project_name/settings.py-tpl
--rw-r--r--   0        0        0      789 2024-06-01 09:52:39.542888 breadslicer-0.0.1/src/opinionated/templates/django/project_template/project_name/urls.py-tpl
--rw-r--r--   0        0        0      428 2024-06-01 09:52:39.542888 breadslicer-0.0.1/src/opinionated/templates/django/project_template/project_name/wsgi.py-tpl
--rw-r--r--   0        0        0      929 2024-06-01 09:52:39.542888 breadslicer-0.0.1/src/opinionated/templates/doc_conf/conf.py
--rw-r--r--   0        0        0        0 2024-06-01 09:52:39.542888 breadslicer-0.0.1/src/opinionated/templates/flask/__init__.py
--rw-r--r--   0        0        0        0 2024-06-01 09:52:39.542888 breadslicer-0.0.1/src/opinionated/templates/flask/py.typed
--rw-r--r--   0        0        0        0 2024-06-01 09:52:39.542888 breadslicer-0.0.1/src/opinionated/templates/flat/__init__.py
--rwxr-xr-x   0        0        0     1844 2024-06-01 09:52:39.542888 breadslicer-0.0.1/src/opinionated/templates/flat/main.py
--rw-r--r--   0        0        0        0 2024-06-01 09:52:39.542888 breadslicer-0.0.1/src/opinionated/templates/flat/py.typed
--rw-r--r--   0        0        0       75 2024-06-01 09:52:39.542888 breadslicer-0.0.1/src/opinionated/templates/poetry.toml
--rw-r--r--   0        0        0        0 2024-06-01 09:52:39.542888 breadslicer-0.0.1/src/opinionated/templates/py.typed
--rw-r--r--   0        0        0     1617 2024-06-01 09:52:39.542888 breadslicer-0.0.1/src/opinionated/templates/pyproject.toml
--rwxr-xr-x   0        0        0       23 2024-06-01 09:52:39.542888 breadslicer-0.0.1/src/opinionated/templates/scripts/build.sh
--rwxr-xr-x   0        0        0      118 2024-06-01 09:52:39.542888 breadslicer-0.0.1/src/opinionated/templates/scripts/install_full_pkg.sh
--rwxr-xr-x   0        0        0       30 2024-06-01 09:52:39.542888 breadslicer-0.0.1/src/opinionated/templates/scripts/release.sh
--rwxr-xr-x   0        0        0       95 2024-06-01 09:52:39.542888 breadslicer-0.0.1/src/opinionated/templates/scripts/tests.sh
--rwxr-xr-x   0        0        0       56 2024-06-01 09:52:39.542888 breadslicer-0.0.1/src/opinionated/templates/scripts/verify.sh
--rw-r--r--   0        0        0        0 2024-06-01 09:52:39.542888 breadslicer-0.0.1/src/opinionated/templates/src/{{project_slug}}/__init__.py
--rwxr-xr-x   0        0        0     1844 2024-06-01 09:52:39.542888 breadslicer-0.0.1/src/opinionated/templates/src/{{project_slug}}/main.py
--rw-r--r--   0        0        0        0 2024-06-01 09:52:39.542888 breadslicer-0.0.1/src/opinionated/templates/src/{{project_slug}}/py.typed
--rw-r--r--   0        0        0        0 2024-06-01 09:52:39.542888 breadslicer-0.0.1/src/opinionated/templates/tests/__init__.py
--rw-r--r--   0        0        0      178 2024-06-01 09:52:39.542888 breadslicer-0.0.1/src/opinionated/templates/tests/test_dummy.py
--rw-r--r--   0        0        0    10349 1970-01-01 00:00:00.000000 breadslicer-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     9858 2024-06-01 16:57:48.639838 breadslicer-0.0.2/README.md
+-rw-r--r--   0        0        0     1443 2024-06-01 16:57:48.640838 breadslicer-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-06-01 16:57:48.680838 breadslicer-0.0.2/src/breadslicer/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-01 16:57:48.680838 breadslicer-0.0.2/src/breadslicer/application/__init__.py
+-rw-r--r--   0        0        0     3019 2024-06-01 16:57:48.641838 breadslicer-0.0.2/src/breadslicer/application/app.py
+-rw-r--r--   0        0        0     1950 2024-06-01 16:57:48.641838 breadslicer-0.0.2/src/breadslicer/application/renderer.py
+-rw-r--r--   0        0        0     1849 2024-06-01 16:57:48.641838 breadslicer-0.0.2/src/breadslicer/application/slice.py
+-rw-r--r--   0        0        0        0 2024-06-01 16:57:48.681838 breadslicer-0.0.2/src/breadslicer/components/__init__.py
+-rw-r--r--   0        0        0      346 2024-06-01 16:57:48.641838 breadslicer-0.0.2/src/breadslicer/components/base.py
+-rw-r--r--   0        0        0      655 2024-06-01 16:57:48.641838 breadslicer-0.0.2/src/breadslicer/components/choice.py
+-rw-r--r--   0        0        0      494 2024-06-01 16:57:48.642838 breadslicer-0.0.2/src/breadslicer/components/confirm.py
+-rw-r--r--   0        0        0      476 2024-06-01 16:57:48.642838 breadslicer-0.0.2/src/breadslicer/components/editor.py
+-rw-r--r--   0        0        0      516 2024-06-01 16:57:48.642838 breadslicer-0.0.2/src/breadslicer/components/multiple_choice.py
+-rw-r--r--   0        0        0      473 2024-06-01 16:57:48.642838 breadslicer-0.0.2/src/breadslicer/components/password.py
+-rw-r--r--   0        0        0     1195 2024-06-01 16:57:48.642838 breadslicer-0.0.2/src/breadslicer/components/text.py
+-rwxr-xr-x   0        0        0     1823 2024-06-01 16:57:48.642838 breadslicer-0.0.2/src/breadslicer/main.py
+-rw-r--r--   0        0        0        0 2024-06-01 16:57:48.685838 breadslicer-0.0.2/src/breadslicer/py.typed
+-rw-r--r--   0        0        0        0 2024-06-01 16:57:48.685838 breadslicer-0.0.2/src/breadslicer/utility/__init__.py
+-rw-r--r--   0        0        0      349 2024-06-01 16:57:48.642838 breadslicer-0.0.2/src/breadslicer/utility/abstractdataclass.py
+-rw-r--r--   0        0        0     1841 2024-06-01 16:57:48.642838 breadslicer-0.0.2/src/breadslicer/utility/command.py
+-rw-r--r--   0        0        0      486 2024-06-01 16:57:48.642838 breadslicer-0.0.2/src/breadslicer/utility/fs.py
+-rw-r--r--   0        0        0      274 2024-06-01 16:57:48.642838 breadslicer-0.0.2/src/breadslicer/utility/git.py
+-rw-r--r--   0        0        0        0 2024-06-01 16:57:48.685838 breadslicer-0.0.2/src/opinionated/__init__.py
+-rw-r--r--   0        0        0     2975 2024-06-01 16:57:48.642838 breadslicer-0.0.2/src/opinionated/bread.py
+-rw-r--r--   0        0        0     3231 2024-06-01 16:57:48.643838 breadslicer-0.0.2/src/opinionated/cleanup.py
+-rw-r--r--   0        0        0     1296 2024-06-01 16:57:48.643838 breadslicer-0.0.2/src/opinionated/dependencies.py
+-rw-r--r--   0        0        0      263 2024-06-01 16:57:48.643838 breadslicer-0.0.2/src/opinionated/includes/Dockerfile.alpine
+-rw-r--r--   0        0        0      334 2024-06-01 16:57:48.643838 breadslicer-0.0.2/src/opinionated/includes/Dockerfile.debian
+-rw-r--r--   0        0        0     1302 2024-06-01 16:57:48.643838 breadslicer-0.0.2/src/opinionated/includes/Dockerfile.python
+-rw-r--r--   0        0        0      339 2024-06-01 16:57:48.643838 breadslicer-0.0.2/src/opinionated/includes/Dockerfile.slim
+-rw-r--r--   0        0        0     2905 2024-06-01 16:57:48.643838 breadslicer-0.0.2/src/opinionated/includes/app.gitlab-ci.yml
+-rw-r--r--   0        0        0     1917 2024-06-01 16:57:48.643838 breadslicer-0.0.2/src/opinionated/includes/lib.gitlab-ci.yml
+-rw-r--r--   0        0        0     2259 2024-06-01 16:57:48.643838 breadslicer-0.0.2/src/opinionated/includes/utils.gitlab-ci.yml
+-rw-r--r--   0        0        0      124 2024-06-01 16:57:48.643838 breadslicer-0.0.2/src/opinionated/project_types.py
+-rw-r--r--   0        0        0        0 2024-06-01 16:57:48.685838 breadslicer-0.0.2/src/opinionated/py.typed
+-rw-r--r--   0        0        0     4512 2024-06-01 16:57:48.643838 breadslicer-0.0.2/src/opinionated/questions.py
+-rw-r--r--   0        0        0     2169 2024-06-01 16:57:48.643838 breadslicer-0.0.2/src/opinionated/templates/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0       61 2024-06-01 16:57:48.643838 breadslicer-0.0.2/src/opinionated/templates/.dockerignore
+-rw-r--r--   0        0        0     1298 2024-06-01 16:57:48.644838 breadslicer-0.0.2/src/opinionated/templates/.envrc
+-rw-r--r--   0        0        0      121 2024-06-01 16:57:48.644838 breadslicer-0.0.2/src/opinionated/templates/.flake8
+-rw-r--r--   0        0        0        0 2024-06-01 16:57:48.685838 breadslicer-0.0.2/src/opinionated/templates/.github/workflows/.keep
+-rw-r--r--   0        0        0      208 2024-06-01 16:57:48.644838 breadslicer-0.0.2/src/opinionated/templates/.gitignore
+-rw-r--r--   0        0        0        0 2024-06-01 16:57:48.685838 breadslicer-0.0.2/src/opinionated/templates/.gitlab/.keep
+-rw-r--r--   0        0        0      146 2024-06-01 16:57:48.644838 breadslicer-0.0.2/src/opinionated/templates/.gitlab-ci.yml
+-rw-r--r--   0        0        0      186 2024-06-01 16:57:48.644838 breadslicer-0.0.2/src/opinionated/templates/.pre-commit-config.yaml
+-rwxr-xr-x   0        0        0     3420 2024-06-01 16:57:48.644838 breadslicer-0.0.2/src/opinionated/templates/.print_help.py
+-rw-r--r--   0        0        0      685 2024-06-01 16:57:48.644838 breadslicer-0.0.2/src/opinionated/templates/.vscode/extensions.json
+-rw-r--r--   0        0        0     2666 2024-06-01 16:57:48.644838 breadslicer-0.0.2/src/opinionated/templates/.vscode/launch.json
+-rw-r--r--   0        0        0      643 2024-06-01 16:57:48.644838 breadslicer-0.0.2/src/opinionated/templates/.vscode/settings.json
+-rw-r--r--   0        0        0     1238 2024-06-01 16:57:48.644838 breadslicer-0.0.2/src/opinionated/templates/.vscode/tasks.json
+-rw-r--r--   0        0        0      211 2024-06-01 16:57:48.644838 breadslicer-0.0.2/src/opinionated/templates/Dockerfile
+-rw-r--r--   0        0        0     4888 2024-06-01 16:57:48.644838 breadslicer-0.0.2/src/opinionated/templates/Makefile
+-rw-r--r--   0        0        0        0 2024-06-01 16:57:48.685838 breadslicer-0.0.2/src/opinionated/templates/README.md
+-rwxr-xr-x   0        0        0      674 2024-06-01 16:57:48.645838 breadslicer-0.0.2/src/opinionated/templates/django/project_template/manage.py-tpl
+-rw-r--r--   0        0        0        0 2024-06-01 16:57:48.685838 breadslicer-0.0.2/src/opinionated/templates/django/project_template/project_name/__init__.py-tpl
+-rw-r--r--   0        0        0      428 2024-06-01 16:57:48.645838 breadslicer-0.0.2/src/opinionated/templates/django/project_template/project_name/asgi.py-tpl
+-rw-r--r--   0        0        0     3390 2024-06-01 16:57:48.645838 breadslicer-0.0.2/src/opinionated/templates/django/project_template/project_name/settings.py-tpl
+-rw-r--r--   0        0        0      789 2024-06-01 16:57:48.645838 breadslicer-0.0.2/src/opinionated/templates/django/project_template/project_name/urls.py-tpl
+-rw-r--r--   0        0        0      428 2024-06-01 16:57:48.645838 breadslicer-0.0.2/src/opinionated/templates/django/project_template/project_name/wsgi.py-tpl
+-rw-r--r--   0        0        0      929 2024-06-01 16:57:48.645838 breadslicer-0.0.2/src/opinionated/templates/doc_conf/conf.py
+-rw-r--r--   0        0        0        0 2024-06-01 16:57:48.686838 breadslicer-0.0.2/src/opinionated/templates/flask/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-01 16:57:48.686838 breadslicer-0.0.2/src/opinionated/templates/flask/py.typed
+-rw-r--r--   0        0        0        0 2024-06-01 16:57:48.686838 breadslicer-0.0.2/src/opinionated/templates/flat/__init__.py
+-rwxr-xr-x   0        0        0     1844 2024-06-01 16:57:48.645838 breadslicer-0.0.2/src/opinionated/templates/flat/main.py
+-rw-r--r--   0        0        0        0 2024-06-01 16:57:48.686838 breadslicer-0.0.2/src/opinionated/templates/flat/py.typed
+-rw-r--r--   0        0        0       75 2024-06-01 16:57:48.645838 breadslicer-0.0.2/src/opinionated/templates/poetry.toml
+-rw-r--r--   0        0        0        0 2024-06-01 16:57:48.686838 breadslicer-0.0.2/src/opinionated/templates/py.typed
+-rw-r--r--   0        0        0     1617 2024-06-01 16:57:48.645838 breadslicer-0.0.2/src/opinionated/templates/pyproject.toml
+-rwxr-xr-x   0        0        0       23 2024-06-01 16:57:48.646838 breadslicer-0.0.2/src/opinionated/templates/scripts/build.sh
+-rwxr-xr-x   0        0        0      118 2024-06-01 16:57:48.646838 breadslicer-0.0.2/src/opinionated/templates/scripts/install_full_pkg.sh
+-rwxr-xr-x   0        0        0       30 2024-06-01 16:57:48.646838 breadslicer-0.0.2/src/opinionated/templates/scripts/release.sh
+-rwxr-xr-x   0        0        0       95 2024-06-01 16:57:48.646838 breadslicer-0.0.2/src/opinionated/templates/scripts/tests.sh
+-rwxr-xr-x   0        0        0       56 2024-06-01 16:57:48.646838 breadslicer-0.0.2/src/opinionated/templates/scripts/verify.sh
+-rw-r--r--   0        0        0        0 2024-06-01 16:57:48.686838 breadslicer-0.0.2/src/opinionated/templates/src/{{project_slug}}/__init__.py
+-rwxr-xr-x   0        0        0     1844 2024-06-01 16:57:48.646838 breadslicer-0.0.2/src/opinionated/templates/src/{{project_slug}}/main.py
+-rw-r--r--   0        0        0        0 2024-06-01 16:57:48.686838 breadslicer-0.0.2/src/opinionated/templates/src/{{project_slug}}/py.typed
+-rw-r--r--   0        0        0        0 2024-06-01 16:57:48.686838 breadslicer-0.0.2/src/opinionated/templates/tests/__init__.py
+-rw-r--r--   0        0        0      178 2024-06-01 16:57:48.646838 breadslicer-0.0.2/src/opinionated/templates/tests/test_dummy.py
+-rw-r--r--   0        0        0    10578 1970-01-01 00:00:00.000000 breadslicer-0.0.2/PKG-INFO
```

### Comparing `breadslicer-0.0.1/README.md` & `breadslicer-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.1/pyproject.toml` & `breadslicer-0.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 [tool.poetry]
 name = "breadslicer"
-version = "0.0.1"
+version = "0.0.2"
 description = "Commandline utililty to create python projects from templates"
 authors = ["Morten Rasmussen <netrom1337@gmail.com>"]
 readme = "README.md"
+homepage = "https://gitlab.com/mindsweeper/open-source/breadslicer"
+documentation = "https://mindsweeper.gitlab.io/open-source/breadslicer/"
+repository = "https://gitlab.com/mindsweeper/open-source/breadslicer"
 
 packages = [
     { include = "breadslicer", from="src"},
     { include = "opinionated", from="src"},
 ]
 
 [tool.poetry.scripts]
```

### Comparing `breadslicer-0.0.1/src/breadslicer/application/app.py` & `breadslicer-0.0.2/src/breadslicer/application/app.py`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.1/src/breadslicer/application/renderer.py` & `breadslicer-0.0.2/src/breadslicer/application/renderer.py`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.1/src/breadslicer/application/slice.py` & `breadslicer-0.0.2/src/breadslicer/application/slice.py`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.1/src/breadslicer/components/choice.py` & `breadslicer-0.0.2/src/breadslicer/components/choice.py`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.1/src/breadslicer/components/multiple_choice.py` & `breadslicer-0.0.2/src/breadslicer/components/multiple_choice.py`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.1/src/breadslicer/components/text.py` & `breadslicer-0.0.2/src/breadslicer/components/text.py`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.1/src/breadslicer/main.py` & `breadslicer-0.0.2/src/breadslicer/main.py`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.1/src/breadslicer/utility/command.py` & `breadslicer-0.0.2/src/breadslicer/utility/command.py`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.1/src/opinionated/bread.py` & `breadslicer-0.0.2/src/opinionated/bread.py`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.1/src/opinionated/cleanup.py` & `breadslicer-0.0.2/src/opinionated/cleanup.py`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.1/src/opinionated/dependencies.py` & `breadslicer-0.0.2/src/opinionated/dependencies.py`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.1/src/opinionated/includes/Dockerfile.python` & `breadslicer-0.0.2/src/opinionated/includes/Dockerfile.python`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.1/src/opinionated/includes/app.gitlab-ci.yml` & `breadslicer-0.0.2/src/opinionated/includes/app.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.1/src/opinionated/includes/lib.gitlab-ci.yml` & `breadslicer-0.0.2/src/opinionated/includes/lib.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.1/src/opinionated/includes/utils.gitlab-ci.yml` & `breadslicer-0.0.2/src/opinionated/includes/utils.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.1/src/opinionated/questions.py` & `breadslicer-0.0.2/src/opinionated/questions.py`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.1/src/opinionated/templates/.devcontainer/devcontainer.json` & `breadslicer-0.0.2/src/opinionated/templates/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.1/src/opinionated/templates/.envrc` & `breadslicer-0.0.2/src/opinionated/templates/.envrc`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.1/src/opinionated/templates/.print_help.py` & `breadslicer-0.0.2/src/opinionated/templates/.print_help.py`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.1/src/opinionated/templates/.vscode/extensions.json` & `breadslicer-0.0.2/src/opinionated/templates/.vscode/extensions.json`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.1/src/opinionated/templates/.vscode/launch.json` & `breadslicer-0.0.2/src/opinionated/templates/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.1/src/opinionated/templates/.vscode/settings.json` & `breadslicer-0.0.2/src/opinionated/templates/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.1/src/opinionated/templates/.vscode/tasks.json` & `breadslicer-0.0.2/src/opinionated/templates/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.1/src/opinionated/templates/Makefile` & `breadslicer-0.0.2/src/opinionated/templates/Makefile`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.1/src/opinionated/templates/django/project_template/manage.py-tpl` & `breadslicer-0.0.2/src/opinionated/templates/django/project_template/manage.py-tpl`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.1/src/opinionated/templates/django/project_template/project_name/settings.py-tpl` & `breadslicer-0.0.2/src/opinionated/templates/django/project_template/project_name/settings.py-tpl`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.1/src/opinionated/templates/django/project_template/project_name/urls.py-tpl` & `breadslicer-0.0.2/src/opinionated/templates/django/project_template/project_name/urls.py-tpl`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.1/src/opinionated/templates/doc_conf/conf.py` & `breadslicer-0.0.2/src/opinionated/templates/doc_conf/conf.py`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.1/src/opinionated/templates/flat/main.py` & `breadslicer-0.0.2/src/opinionated/templates/flat/main.py`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.1/src/opinionated/templates/pyproject.toml` & `breadslicer-0.0.2/src/opinionated/templates/pyproject.toml`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.1/src/opinionated/templates/src/{{project_slug}}/main.py` & `breadslicer-0.0.2/src/opinionated/templates/src/{{project_slug}}/main.py`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.1/PKG-INFO` & `breadslicer-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: breadslicer
-Version: 0.0.1
+Version: 0.0.2
 Summary: Commandline utililty to create python projects from templates
+Home-page: https://gitlab.com/mindsweeper/open-source/breadslicer
 Author: Morten Rasmussen
 Author-email: netrom1337@gmail.com
 Requires-Python: >=3.10.7,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: inquirer (>=3.2.4,<4.0.0)
 Requires-Dist: jinja2 (>=3.1.4,<4.0.0)
+Project-URL: Documentation, https://mindsweeper.gitlab.io/open-source/breadslicer/
+Project-URL: Repository, https://gitlab.com/mindsweeper/open-source/breadslicer
 Description-Content-Type: text/markdown
 
 
 # Breadslicer
 
 Breadslicer is a opinionated python project template engine. Which can be
 programmed with a set of function and methods and overloading classes.
```

