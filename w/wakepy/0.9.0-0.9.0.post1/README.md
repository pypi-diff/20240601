# Comparing `tmp/wakepy-0.9.0.tar.gz` & `tmp/wakepy-0.9.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wakepy-0.9.0.tar", last modified: Thu May 30 21:31:53 2024, max compression
+gzip compressed data, was "wakepy-0.9.0.post1.tar", last modified: Sat Jun  1 09:16:36 2024, max compression
```

## Comparing `wakepy-0.9.0.tar` & `wakepy-0.9.0.post1.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:53.440820 wakepy-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-30 21:31:40.000000 wakepy-0.9.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:53.416820 wakepy-0.9.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:53.424820 wakepy-0.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-05-30 21:31:40.000000 wakepy-0.9.0/.github/workflows/build-and-run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-30 21:31:40.000000 wakepy-0.9.0/.github/workflows/publish-a-release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-30 21:31:40.000000 wakepy-0.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-30 21:31:40.000000 wakepy-0.9.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-05-30 21:31:40.000000 wakepy-0.9.0/DEV.md
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-30 21:31:40.000000 wakepy-0.9.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-05-30 21:31:53.440820 wakepy-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-30 21:31:40.000000 wakepy-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:53.424820 wakepy-0.9.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-30 21:31:40.000000 wakepy-0.9.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-30 21:31:40.000000 wakepy-0.9.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:53.424820 wakepy-0.9.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:53.424820 wakepy-0.9.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-05-30 21:31:40.000000 wakepy-0.9.0/docs/source/_static/wakepy-docs.css
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-30 21:31:40.000000 wakepy-0.9.0/docs/source/_static/wakepy-docs.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:53.424820 wakepy-0.9.0/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:40.000000 wakepy-0.9.0/docs/source/_templates/author.html
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-30 21:31:40.000000 wakepy-0.9.0/docs/source/_templates/sbt-sidebar-nav.html
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-30 21:31:40.000000 wakepy-0.9.0/docs/source/api-reference.md
--rw-r--r--   0 runner    (1001) docker     (127)    13097 2024-05-30 21:31:40.000000 wakepy-0.9.0/docs/source/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-30 21:31:40.000000 wakepy-0.9.0/docs/source/cli-api.md
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-05-30 21:31:40.000000 wakepy-0.9.0/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:53.428820 wakepy-0.9.0/docs/source/img/
--rw-r--r--   0 runner    (1001) docker     (127)    19633 2024-05-30 21:31:40.000000 wakepy-0.9.0/docs/source/img/activate-mode-activity-diagram.svg
--rw-r--r--   0 runner    (1001) docker     (127)    34844 2024-05-30 21:31:40.000000 wakepy-0.9.0/docs/source/img/activate-mode-using-method-activity-diagram.svg
--rw-r--r--   0 runner    (1001) docker     (127)    35437 2024-05-30 21:31:40.000000 wakepy-0.9.0/docs/source/img/mode-activity-diagram.svg
--rw-r--r--   0 runner    (1001) docker     (127)    18172 2024-05-30 21:31:40.000000 wakepy-0.9.0/docs/source/img/mode-state-diagram.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-05-30 21:31:40.000000 wakepy-0.9.0/docs/source/index.md
--rw-r--r--   0 runner    (1001) docker     (127)    14784 2024-05-30 21:31:40.000000 wakepy-0.9.0/docs/source/methods-reference.md
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-30 21:31:40.000000 wakepy-0.9.0/docs/source/migration.md
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-05-30 21:31:40.000000 wakepy-0.9.0/docs/source/modes.md
--rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-05-30 21:31:40.000000 wakepy-0.9.0/docs/source/test-manually.md
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-30 21:31:40.000000 wakepy-0.9.0/docs/source/tests-and-ci.md
--rw-r--r--   0 runner    (1001) docker     (127)     8509 2024-05-30 21:31:40.000000 wakepy-0.9.0/docs/source/user-guide.md
--rw-r--r--   0 runner    (1001) docker     (127)     7954 2024-05-30 21:31:40.000000 wakepy-0.9.0/docs/source/wakepy-mode-lifecycle.md
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-05-30 21:31:40.000000 wakepy-0.9.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:53.428820 wakepy-0.9.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-30 21:31:40.000000 wakepy-0.9.0/requirements/requirements-check.txt
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-30 21:31:40.000000 wakepy-0.9.0/requirements/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-30 21:31:40.000000 wakepy-0.9.0/requirements/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-30 21:31:40.000000 wakepy-0.9.0/requirements/requirements-mypy.txt
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-30 21:31:40.000000 wakepy-0.9.0/requirements/requirements-test.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:53.428820 wakepy-0.9.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-30 21:31:40.000000 wakepy-0.9.0/scripts/example-test.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 21:31:53.440820 wakepy-0.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:53.420820 wakepy-0.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:53.428820 wakepy-0.9.0/src/wakepy/
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-30 21:31:53.000000 wakepy-0.9.0/src/wakepy/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:53.432820 wakepy-0.9.0/src/wakepy/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9278 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/core/activationresult.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    13527 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/core/dbus.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/core/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (127)    21036 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/core/method.py
--rw-r--r--   0 runner    (1001) docker     (127)    22236 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/core/mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/core/platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     8990 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/core/prioritization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/core/strenum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:53.432820 wakepy-0.9.0/src/wakepy/dbus_adapters/
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/dbus_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/dbus_adapters/jeepney.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:53.436820 wakepy-0.9.0/src/wakepy/methods/
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/methods/_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8362 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/methods/freedesktop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/methods/gnome.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/methods/macos.py
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/methods/windows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:53.436820 wakepy-0.9.0/src/wakepy/modes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/modes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/modes/keep.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:53.440820 wakepy-0.9.0/src/wakepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-05-30 21:31:53.000000 wakepy-0.9.0/src/wakepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-05-30 21:31:53.000000 wakepy-0.9.0/src/wakepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 21:31:53.000000 wakepy-0.9.0/src/wakepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-30 21:31:53.000000 wakepy-0.9.0/src/wakepy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-30 21:31:53.000000 wakepy-0.9.0/src/wakepy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-30 21:31:53.000000 wakepy-0.9.0/src/wakepy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-30 21:31:40.000000 wakepy-0.9.0/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:53.436820 wakepy-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:53.436820 wakepy-0.9.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6954 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/integration/dbus_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     7382 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/integration/test_dbus_adapters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/tox_build_wakepy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:53.436820 wakepy-0.9.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:53.440820 wakepy-0.9.0/tests/unit/test_core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test_core/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    15382 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test_core/test_activationresult.py
--rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test_core/test_calls.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test_core/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test_core/test_dbus.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test_core/test_heartbeat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:53.440820 wakepy-0.9.0/tests/unit/test_core/test_method/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test_core/test_method/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19101 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test_core/test_method/test_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test_core/test_method/test_method.py
--rw-r--r--   0 runner    (1001) docker     (127)    14463 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test_core/test_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test_core/test_platform.py
--rw-r--r--   0 runner    (1001) docker     (127)    14593 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test_core/test_prioritization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test_core/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test_core/test_strenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test_core/testmethods.py
--rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:53.440820 wakepy-0.9.0/tests/unit/test_methods/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test_methods/test_freedesktop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test_methods/test_gnome.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test_methods/test_macos.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test_methods/test_windows.py
--rw-r--r--   0 runner    (1001) docker     (127)     5908 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test_modes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-05-30 21:31:40.000000 wakepy-0.9.0/tox.ini
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-05-30 21:31:40.000000 wakepy-0.9.0/toxfile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:16:36.291001 wakepy-0.9.0.post1/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:16:36.267001 wakepy-0.9.0.post1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:16:36.275001 wakepy-0.9.0.post1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/.github/workflows/build-and-run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/.github/workflows/publish-a-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/DEV.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12602 2024-06-01 09:16:36.291001 wakepy-0.9.0.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10012 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:16:36.275001 wakepy-0.9.0.post1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:16:36.275001 wakepy-0.9.0.post1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:16:36.275001 wakepy-0.9.0.post1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/docs/source/_static/wakepy-docs.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/docs/source/_static/wakepy-docs.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:16:36.275001 wakepy-0.9.0.post1/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/docs/source/_templates/author.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/docs/source/_templates/sbt-sidebar-nav.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/docs/source/api-reference.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13230 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/docs/source/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/docs/source/cli-api.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:16:36.279001 wakepy-0.9.0.post1/docs/source/img/
+-rw-r--r--   0 runner    (1001) docker     (127)    19633 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/docs/source/img/activate-mode-activity-diagram.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    34844 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/docs/source/img/activate-mode-using-method-activity-diagram.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    35437 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/docs/source/img/mode-activity-diagram.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    18172 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/docs/source/img/mode-state-diagram.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/docs/source/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12913 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/docs/source/methods-reference.md
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/docs/source/migration.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4861 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/docs/source/modes.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/docs/source/test-manually.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/docs/source/tests-and-ci.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8461 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/docs/source/user-guide.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7954 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/docs/source/wakepy-mode-lifecycle.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:16:36.279001 wakepy-0.9.0.post1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/requirements/requirements-check.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/requirements/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/requirements/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/requirements/requirements-mypy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/requirements/requirements-test.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:16:36.279001 wakepy-0.9.0.post1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/scripts/example-test.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 09:16:36.291001 wakepy-0.9.0.post1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:16:36.271001 wakepy-0.9.0.post1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:16:36.279001 wakepy-0.9.0.post1/src/wakepy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/src/wakepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/src/wakepy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-06-01 09:16:36.000000 wakepy-0.9.0.post1/src/wakepy/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:16:36.283001 wakepy-0.9.0.post1/src/wakepy/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/src/wakepy/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9278 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/src/wakepy/core/activationresult.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/src/wakepy/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13527 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/src/wakepy/core/dbus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/src/wakepy/core/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21036 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/src/wakepy/core/method.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22236 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/src/wakepy/core/mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/src/wakepy/core/platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8990 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/src/wakepy/core/prioritization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/src/wakepy/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/src/wakepy/core/strenum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:16:36.283001 wakepy-0.9.0.post1/src/wakepy/dbus_adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/src/wakepy/dbus_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/src/wakepy/dbus_adapters/jeepney.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:16:36.287001 wakepy-0.9.0.post1/src/wakepy/methods/
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/src/wakepy/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/src/wakepy/methods/_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8362 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/src/wakepy/methods/freedesktop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/src/wakepy/methods/gnome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/src/wakepy/methods/macos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/src/wakepy/methods/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:16:36.287001 wakepy-0.9.0.post1/src/wakepy/modes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/src/wakepy/modes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7109 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/src/wakepy/modes/keep.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/src/wakepy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:16:36.291001 wakepy-0.9.0.post1/src/wakepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12602 2024-06-01 09:16:36.000000 wakepy-0.9.0.post1/src/wakepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-06-01 09:16:36.000000 wakepy-0.9.0.post1/src/wakepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 09:16:36.000000 wakepy-0.9.0.post1/src/wakepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-06-01 09:16:36.000000 wakepy-0.9.0.post1/src/wakepy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-06-01 09:16:36.000000 wakepy-0.9.0.post1/src/wakepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-06-01 09:16:36.000000 wakepy-0.9.0.post1/src/wakepy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:16:36.287001 wakepy-0.9.0.post1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:16:36.287001 wakepy-0.9.0.post1/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6954 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/tests/integration/dbus_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7382 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/tests/integration/test_dbus_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/tests/tox_build_wakepy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:16:36.287001 wakepy-0.9.0.post1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/tests/unit/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/tests/unit/test__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:16:36.291001 wakepy-0.9.0.post1/tests/unit/test_core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/tests/unit/test_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/tests/unit/test_core/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15382 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/tests/unit/test_core/test_activationresult.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/tests/unit/test_core/test_calls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/tests/unit/test_core/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/tests/unit/test_core/test_dbus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/tests/unit/test_core/test_heartbeat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:16:36.291001 wakepy-0.9.0.post1/tests/unit/test_core/test_method/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/tests/unit/test_core/test_method/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19101 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/tests/unit/test_core/test_method/test_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/tests/unit/test_core/test_method/test_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14463 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/tests/unit/test_core/test_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/tests/unit/test_core/test_platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14593 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/tests/unit/test_core/test_prioritization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/tests/unit/test_core/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/tests/unit/test_core/test_strenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/tests/unit/test_core/testmethods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/tests/unit/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:16:36.291001 wakepy-0.9.0.post1/tests/unit/test_methods/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/tests/unit/test_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/tests/unit/test_methods/test_freedesktop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/tests/unit/test_methods/test_gnome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/tests/unit/test_methods/test_macos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/tests/unit/test_methods/test_windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5908 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/tests/unit/test_modes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-06-01 09:16:19.000000 wakepy-0.9.0.post1/toxfile.py
```

### Comparing `wakepy-0.9.0/.github/workflows/build-and-run-tests.yml` & `wakepy-0.9.0.post1/.github/workflows/build-and-run-tests.yml`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/.github/workflows/publish-a-release.yml` & `wakepy-0.9.0.post1/.github/workflows/publish-a-release.yml`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/DEV.md` & `wakepy-0.9.0.post1/DEV.md`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/LICENSE.txt` & `wakepy-0.9.0.post1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/docs/Makefile` & `wakepy-0.9.0.post1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/docs/make.bat` & `wakepy-0.9.0.post1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/docs/source/_static/wakepy-docs.css` & `wakepy-0.9.0.post1/docs/source/_static/wakepy-docs.css`

 * *Files 14% similar despite different names*

```diff
@@ -5,39 +5,53 @@
 html[data-theme=light] {
     /* the contents directive */
     --wakepy-color-contents-bg: #f9f9fb;
     --wakepy-color-contents-border: #eff0f0;
     --wakepy-color-inline-code: #d70936;
     --wakepy-color-code-block-bg: #fcfcfd;
     --wakepy-color-code-block-border: #d1d5da;
+    --wakepy-table-color-header-bottom-border: #f6f6f6;
     /* tables */
     --wakepy-table-color-header-bg: #f6f6f6;
     --wakepy-table-color-bg: #fff;
     --wakepy-table-color-border: #ddd;
     /* Regular links color */
     --pst-color-link: #0250e3;
     /* Navigation links color */
     --pst-color-primary: #0250e3;
+    /* override table row coloring (odd rows) */
+    --pst-color-table-row-zebra-low-bg: rgb(255, 255, 255) !important;
+    /* override table row coloring (even rows) */
+    --pst-color-table-row-zebra-high-bg: rgb(255, 255, 255) !important;
+    /* override table row hover background color */
+    --pst-color-table-row-hover-bg: #fafafaff !important;
 }
 
 
 html[data-theme=dark] {
     /* for explanations, refer to the light theme definitions */
     --wakepy-color-contents-bg: #191825;
     --wakepy-color-contents-border: #293342;
     --wakepy-color-inline-code:#dd7886;
     --wakepy-color-code-block-bg: #272822;
     --wakepy-color-code-block-border: #3c3d2e;
-    --wakepy-table-color-header-bg: #29313d;
+    --wakepy-table-color-header-bg: #222832ff;
     --wakepy-table-color-bg: #0f1216;
     --wakepy-table-color-border: #29313d;
+    --wakepy-table-color-header-bottom-border: #29313d;
     /* Regular links color */
     --pst-color-link: #6e91d8;
     /* Navigation links color */
     --pst-color-primary: #6e91d8;
+    /* override table row coloring (odd rows) */
+    --pst-color-table-row-zebra-low-bg: #121212ff !important;
+    /* override table row coloring (even rows) */
+    --pst-color-table-row-zebra-high-bg: #121212ff !important;
+    /* override table row hover background color */
+    --pst-color-table-row-hover-bg: #171717ff !important;
 }
 
 nav.contents  {
     /* For the "contents" directive block */
     background: var(--wakepy-color-contents-bg) !important;
     border-color: var(--wakepy-color-contents-border) !important;
     box-shadow: none !important;
@@ -123,7 +137,13 @@
 .wakepy-table td:first-child {
   vertical-align: top; /* Align text to the top in the first column */
 }
 
 .wakepy-table td {
   background-color: var(--wakepy-table-color-bg);
 }
+
+/* all tables.  */
+thead > tr {
+  background-color: var(--wakepy-table-color-header-bg) !important;
+  border-bottom: 1px solid var(--wakepy-table-color-header-bottom-border) !important;
+}
```

### Comparing `wakepy-0.9.0/docs/source/_static/wakepy-docs.js` & `wakepy-0.9.0.post1/docs/source/_static/wakepy-docs.js`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/docs/source/_templates/sbt-sidebar-nav.html` & `wakepy-0.9.0.post1/docs/source/_templates/sbt-sidebar-nav.html`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/docs/source/api-reference.md` & `wakepy-0.9.0.post1/docs/source/api-reference.md`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/docs/source/changelog.md` & `wakepy-0.9.0.post1/docs/source/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 # Changelog
 
+## wakepy 0.9.0.post1
+🗓️ 2024-06-01
+
+### 📖 Documentation
+- Update docs and README after 0.8.0 & 0.9.0 releases ([#331](https://github.com/fohrloop/wakepy/pull/331))
+
+
 ## wakepy 0.9.0
 🗓️ 2024-05-31
 
 ### ✨ Features
-- Support keep.running mode in KDE Plasma 5.12.90 and newer through the [org.freedesktop.PowerManagement](#keep-running-org-freedesktop-powermanagement) method. It may also be used on other DEs which implement this older freedesktop.org D-Bus interface (but not Xcfe). ([#324](https://github.com/fohrloop/wakepy/pull/324))
+- Support keep.running mode in KDE Plasma 5.12.90 and newer through the [org.freedesktop.PowerManagement](#org-freedesktop-powermanagement) method. It may also be used on other DEs which implement this older freedesktop.org D-Bus interface (but not Xcfe). ([#324](https://github.com/fohrloop/wakepy/pull/324))
 - Cooler CLI spinner ([#309](https://github.com/fohrloop/wakepy/pull/309), [#323](https://github.com/fohrloop/wakepy/pull/323))
 
 ### 📖 Documentation
-- Document that the [org.freedesktop.ScreenSaver](keep-presenting-org-freedesktop-screensaver) method for keep.presenting mode also supports KDE Plasma. ([#324](https://github.com/fohrloop/wakepy/pull/324))
+- Document that the [org.freedesktop.ScreenSaver](org-freedesktop-screensaver) method for keep.presenting mode also supports KDE Plasma. ([#324](https://github.com/fohrloop/wakepy/pull/324))
 - Update dev docs ([#308](https://github.com/fohrloop/wakepy/pull/308))
 - Mention that shell should be restarted for wakepy CLI tool ([#321](https://github.com/fohrloop/wakepy/pull/321))
 - Fix: Supported Platforms table background does not support dark mode ([#316](https://github.com/fohrloop/wakepy/pull/316))
 
 ## wakepy 0.8.0
 🗓️ 2024-05-26
 
 ### 🏆 Highlights
 - This is a basically a complete rewrite of wakepy. It adds support for keep.running mode on Gnome, on-fail action, possibility to control the used methods and their priority, more information about the used methods and the activation process and possibility to exit the mode early. In addition, testing and CI pipelines were updated to ease maintenance.
 
 ### ✨ Features
 - Modes support [on-fail actions](#on-fail-action) ("error", "warn", "pass" or a callable). ([#182](https://github.com/fohrloop/wakepy/pull/182))
 - It is now possible to [select the used wakepy.Methods](#how-to-white-or-blacklist-methods) with `methods` and  `omit` and to [change the priority order](#how-to-control-order-of-methods) of methods with `methods_priority`. ([#75](https://github.com/fohrloop/wakepy/issues/75))
-- Added [org.gnome.SessionManager](#keep-running-org-gnome-sessionmanager) method which adds support for keep.running mode for users with Gnome Desktop Environment. ([#51](https://github.com/fohrloop/wakepy/pull/51), [#138](https://github.com/fohrloop/wakepy/pull/138), [#278](https://github.com/fohrloop/wakepy/pull/278), [#282](https://github.com/fohrloop/wakepy/pull/282))
+- Added [org.gnome.SessionManager](#org-gnome-sessionmanager) method which adds support for keep.running mode for users with Gnome Desktop Environment. ([#51](https://github.com/fohrloop/wakepy/pull/51), [#138](https://github.com/fohrloop/wakepy/pull/138), [#278](https://github.com/fohrloop/wakepy/pull/278), [#282](https://github.com/fohrloop/wakepy/pull/282))
 - {class}`ActivationResult <wakepy.ActivationResult>` objects ([#57](https://github.com/fohrloop/wakepy/pull/57), [#258](https://github.com/fohrloop/wakepy/pull/258), [#270](https://github.com/fohrloop/wakepy/pull/270)) in {attr}`Mode.activation_result <wakepy.Mode.activation_result>` which give more detailed information about the activation process.
 - Possibility to exit from a mode context manager early with {class}`ModeExit <wakepy.ModeExit>`  ([#72](https://github.com/fohrloop/wakepy/pull/72))
 - It's now possible to check the active and used method from the Mode instance using the {attr}`Mode.active_method <wakepy.Mode.active_method>` and  {attr}`Mode.used_method <wakepy.Mode.used_method>` ([#268](https://github.com/fohrloop/wakepy/pull/268))
 - Added possibility to use any dbus python implementation through the {class}`DBusAdapter <wakepy.DBusAdapter>`. By default uses jeepney through {class}`JeepneyDBusAdapter <wakepy.JeepneyDBusAdapter>`  (See: [#45](https://github.com/fohrloop/wakepy/issues/45))
 ### 🚨 Backwards incompatible
 - Removed `set_keepawake` and `unset_keepawake functions` and the `keepawake` context manager. These were deprecated in 0.7.0 and are replaced with the new api: {func}`keep.running() <wakepy.keep.running>` and {func}`keep.presenting() <wakepy.keep.presenting>` context managers. ([#85](https://github.com/fohrloop/wakepy/pull/85))
 - Renamed the CLI argument `-s, --keep-screen-awake` to `-p, --presentation`. The old ones were deprecated in 0.7.0. ([#179](https://github.com/fohrloop/wakepy/pull/179/))
```

### Comparing `wakepy-0.9.0/docs/source/cli-api.md` & `wakepy-0.9.0.post1/docs/source/cli-api.md`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/docs/source/conf.py` & `wakepy-0.9.0.post1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/docs/source/img/activate-mode-activity-diagram.svg` & `wakepy-0.9.0.post1/docs/source/img/activate-mode-activity-diagram.svg`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/docs/source/img/activate-mode-using-method-activity-diagram.svg` & `wakepy-0.9.0.post1/docs/source/img/activate-mode-using-method-activity-diagram.svg`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/docs/source/img/mode-activity-diagram.svg` & `wakepy-0.9.0.post1/docs/source/img/mode-activity-diagram.svg`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/docs/source/img/mode-state-diagram.svg` & `wakepy-0.9.0.post1/docs/source/img/mode-state-diagram.svg`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/docs/source/methods-reference.md` & `wakepy-0.9.0.post1/docs/source/methods-reference.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,70 +1,94 @@
 (wakepy-methods)=
 # Wakepy Methods
 
-
 **What are wakepy Methods?**
-Methods are different ways of entering in (or keeping a) Mode. A Method may support one or more platforms, and may have one or more requirements for software it should be able to talk to or execute. For example, on Linux. using the Inhibit method of the [org.gnome.SessionManager](#keep-running-org-gnome-sessionmanager) D-Bus service is one way of entering  the [`keep.running`](#keep-running-section) mode, and it requires D-Bus and (a certain version of) GNOME. The following methods exist:
-
+Methods are different ways of entering in (or keeping a) Mode. A Method may support one or more platforms, and may have one or more requirements for software it should be able to talk to or execute. For example, on Linux. using the Inhibit method of the [org.gnome.SessionManager](#org-gnome-sessionmanager) D-Bus service is one way of entering  the [`keep.running`](#keep-running-mode) mode, and it requires D-Bus and (a certain version of) GNOME. The following methods exist (⌛: [`keep.running`](#keep-running-mode), 🖥️: [`keep.presenting`](#keep-presenting-mode)): 
 
+| Method                          | Modes |
+| ------------------------------- | ----- |
+| [caffeinate](#macos-caffeinate) | ⌛ 🖥️ |
+| [org.freedesktop.PowerManagement](org-freedesktop-powermanagement) | ⌛ |
+| [org.freedesktop.ScreenSaver](org-freedesktop-screensaver) | 🖥️ |
+| [org.gnome.SessionManager](org-gnome-sessionmanager) | ⌛🖥️ |
+| [SetThreadExecutionState](windows-stes) | ⌛🖥️ |
 
-<!-- using the contents directive https://myst-parser.readthedocs.io/en/latest/syntax/organising_content.html -->
-```{contents}
-:local: True
-:depth: 2
-:class: this-will-duplicate-information-and-it-is-still-useful-here
-```
 
-(keep-running-section)=
-## keep.running
+(macos-caffeinate)=
+## caffeinate
 
-(keep-running-org-gnome-sessionmanager)=
-### org.gnome.SessionManager
-- **Name**: `org.gnome.SessionManager`
-- **Introduced in**: wakepy 0.8.0
-- **How it works**: Uses the [Inhibit](https://lira.no-ip.org:8443/doc/gnome-session/dbus/gnome-session.html#org.gnome.SessionManager.Inhibit) method of [org.gnome.SessionManager](https://lira.no-ip.org:8443/doc/gnome-session/dbus/gnome-session.html#org.gnome.SessionManager) D-Bus service with flag 4 ("Inhibit suspending the session or computer") when activating and saves the returned cookie on the Method instance. Uses the [Uninhibit](https://lira.no-ip.org:8443/doc/gnome-session/dbus/gnome-session.html#org.gnome.SessionManager.Uninhibit) method of the org.gnome.SessionManager with the cookie when deactivating.
+- **Name**: `caffeinate`
+- **Modes**: [`keep.running`](#keep-running-mode), [`keep.presenting`](#keep-presenting-mode)
+- **Introduced in**: wakepy 0.3.0
+- **How it works**: It calls the `caffeinate` command to activate the keep.running mode and add the `-d` flag ("Create an assertion to prevent the display from sleeping.") for keep.presenting mode. See docs at [ss64.com](https://ss64.com/mac/caffeinate.html) or at archives from [developer.apple.com](https://web.archive.org/web/20140604153141/https://developer.apple.com/library/mac/documentation/Darwin/Reference/ManPages/man8/caffeinate.8.html)
 - **Multiprocess safe?**: Yes
 - **What if the process holding the lock dies?**: The lock is automatically removed.
-- **How to check it?**:  You may check the list of inhibitors using the [GetInhibitors](https://lira.no-ip.org:8443/doc/gnome-session/dbus/gnome-session.html#org.gnome.SessionManager.GetInhibitors) method, which gives you list of object paths like `["/org/gnome/SessionManager/Inhibitor20"]`. Then you can use the [GetAppId](https://lira.no-ip.org:8443/doc/gnome-session/dbus/gnome-session.html#org.gnome.SessionManager.Inhibitor.GetAppId), [GetFlags](https://lira.no-ip.org:8443/doc/gnome-session/dbus/gnome-session.html#org.gnome.SessionManager.Inhibitor.GetFlags) and [GetReason](https://lira.no-ip.org:8443/doc/gnome-session/dbus/gnome-session.html#org.gnome.SessionManager.Inhibitor.GetReason) methods on the [org.gnome.SessionManager.Inhibitor](https://lira.no-ip.org:8443/doc/gnome-session/dbus/gnome-session.html#org.gnome.SessionManager.Inhibitor) interface of the listed objects on the org.gnome.SessionManager service to translate that into something meaningful. A good tool for this is [D-Spy](https://apps.gnome.org/Dspy/). Alternatively, you could monitor your inhibit call with [`dbus-monitor`](https://dbus.freedesktop.org/doc/dbus-monitor.1.html).
-- **Requirements**: D-Bus, GNOME Desktop Environment with gnome-session running. The exact version of required GNOME is unknown, but this should work from GNOME 2.24 ([2008-09-23](https://gitlab.gnome.org/GNOME/gnome-session/-/tags/GNOME_SESSION_2_24_0)) onwards. See [version history of org.gnome.SessionManager.xml](https://gitlab.gnome.org/GNOME/gnome-session/-/commits/main/gnome-session/org.gnome.SessionManager.xml). At least [this](https://fedoraproject.org/wiki/Desktop/Whiteboards/InhibitApis) and [this](https://bugzilla.redhat.com/show_bug.cgi?id=529287#c3) mention GNOME 2.24.
-- **Tested on**:  Ubuntu 22.04.3 LTS with GNOME 42.9 ([PR #138](https://github.com/fohrloop/wakepy/pull/138) by [fohrloop](https://github.com/fohrloop/)).
-
-````{admonition} May slow down system if called repeatedly
-:class: warning
-
-If used hundreds or thousands of times, may slow down system. See: [wakepy/#277](https://github.com/fohrloop/wakepy/issues/277)
-````
+- **How to check it?**: You should be able to see a process with a command `/bin/bash caffeinate` or similar associated with it using a task manager.
+- **Requirements**: Mac OS X 10.8 Mountain Lion (July 2012) or newer.
 
 
-(keep-running-org-freedesktop-powermanagement)=
-### org.freedesktop.PowerManagement
+(org-freedesktop-powermanagement)=
+## org.freedesktop.PowerManagement
 - **Name**: `org.freedesktop.PowerManagement`
+- **Modes**: [`keep.running`](#keep-running-mode)
 - **Introduced in**: wakepy 0.9.0
 - **How it works**: Uses the Inhibit method of the org.freedesktop.PowerManagement D-Bus service when activating and saves the returned cookie on the Method instance. Uses UnInhibit method of the same service with the cookie when deactivating. The org.freedesktop.PowerManagement is an obsolete spec, but certain Desktop Environments provide that as the only option for inhibiting the suspend action. The documentation was previously hosted on [freedesktop.org](https://www.freedesktop.org/wiki/Specifications/power-management-spec/) but the links on the page are dead. The spec has three versions: 0.1, 0.2 and 0.3. The 0.3 is not found anywhere but the version 0.2 of the spec can be read in the [Internet Archive](https://web.archive.org/web/20090417010057/http://people.freedesktop.org/~hughsient/temp/power-management-spec-0.2.html)
 - **Multiprocess safe?**: Yes
 - **What if the process holding the lock dies?**: The lock is automatically removed.
 - **How to check it?**:  You may check if there are *any* inhibitors using the HasInhibit method of the `/org/freedesktop/PowerManagement/Inhibit` object on the `org.freedesktop.PowerManagement.Inhibit` interface. Note that updating the inhibit flag from `false` to `true` may take a few seconds. A good tool for this is [D-Spy](https://apps.gnome.org/Dspy/). Alternatively, you could monitor your inhibit call with [`dbus-monitor`](https://dbus.freedesktop.org/doc/dbus-monitor.1.html).
 - **Requirements**: D-Bus + KDE Plasma >=5.12.90 or other DE which implements this older freedesktop D-Bus interface. Exception: Xfce is not supported.
-- **About unsupported DEs** Older versions of KDE Plasma had a bug which also prevented the screenlock/screesaver activation. The bug was fixed in [D11182](https://phabricator.kde.org/D11182), commit  [152400c1b688](https://phabricator.kde.org/R122:152400c1b6880506ee1395011686c2b191f419a0) and was part of the KDE Plasma to 5.12.90 ( = 5.13 Beta) [release](https://kde.org/announcements/changelogs/plasma/5/5.12.5-5.12.90/). This Method is not supported either on Xfce as it has similar bug which prevents also the automatic screenlock/screensaver (See: [xfce4-power-manager/#65](https://gitlab.xfce.org/xfce/xfce4-power-manager/-/issues/65)), hence, wakepy refuses to use org.freedesktop.PowerManagement as method for keep.running mode on KDE < 5.12.90 and on any version of Xfce.
+- **About unsupported DEs** Older versions of KDE Plasma had a bug which also prevented the screenlock/screesaver activation. The bug was fixed in [D11182](https://phabricator.kde.org/D11182), commit  [152400c1b688](https://phabricator.kde.org/R122:152400c1b6880506ee1395011686c2b191f419a0) and was part of the KDE Plasma 5.12.90 ( = 5.13 Beta) [release](https://kde.org/announcements/changelogs/plasma/5/5.12.5-5.12.90/). This Method is not supported either on Xfce as it has similar bug which prevents also the automatic screenlock/screensaver (See: [xfce4-power-manager/#65](https://gitlab.xfce.org/xfce/xfce4-power-manager/-/issues/65)), hence, wakepy refuses to use org.freedesktop.PowerManagement as method for keep.running mode on KDE < 5.12.90 and on any version of Xfce.
 - **Tested on**:  openSUSE 15.5 with KDE Plasma 5.27.9 ([Comment in #310](https://github.com/fohrloop/wakepy/issues/310#issuecomment-2140156882) by [fohrloop](https://github.com/fohrloop/)).
 
+(org-freedesktop-screensaver)=
+## org.freedesktop.ScreenSaver
+- **Name**: `org.freedesktop.ScreenSaver`
+- **Modes**: [`keep.presenting`](#keep-presenting-mode)
+- **Introduced in**: wakepy 0.6.0
+- **How it works**: Uses the Inhibit method of [org.freedesktop.ScreenSaver](https://people.freedesktop.org/~hadess/idle-inhibition-spec/re01.html) D-Bus service when activating and saves the returned cookie on the Method instance. Uses the org.freedesktop.ScreenSaver.UnInhibit method with the cookie when deactivating. The org.freedesktop.ScreenSaver can only be used to prevent idle; that is why there is no "keep.running" mode counterpart.
+- **Multiprocess safe?**: Yes
+- **What if the process holding the lock dies?**: The lock is automatically removed.
+- **How to check it?**:  The org.freedesktop.ScreenSaver does not expose a method for listing the inhibitors, but you could monitor your inhibit call with [`dbus-monitor`](https://dbus.freedesktop.org/doc/dbus-monitor.1.html).
+- **Requirements**: D-Bus, and a [freedesktop.org compliant desktop environment](https://www.freedesktop.org/wiki/Desktops/), which should implement the org.freedesktop.ScreenSaver.Inhibit method.
+- **Tested on**:  Ubuntu 22.04 with GNOME 42.9 ([wakepy/#171](https://github.com/fohrloop/wakepy/pull/171)) and openSUSE 15.5 with KDE Plasma 5.27.9 ([wakepy/#310](https://github.com/fohrloop/wakepy/issues/310#issuecomment-2135512139)) by [fohrloop](https://github.com/fohrloop/).
 
-(keep-running-windows-stes)=
-### SetThreadExecutionState
+
+(org-gnome-sessionmanager)=
+## org.gnome.SessionManager
+- **Name**: `org.gnome.SessionManager`
+- **Modes**: [`keep.running`](#keep-running-mode), [`keep.presenting`](#keep-presenting-mode)
+- **Introduced in**: wakepy 0.8.0
+- **How it works**: Uses the [Inhibit](https://lira.no-ip.org:8443/doc/gnome-session/dbus/gnome-session.html#org.gnome.SessionManager.Inhibit) method of [org.gnome.SessionManager](https://lira.no-ip.org:8443/doc/gnome-session/dbus/gnome-session.html#org.gnome.SessionManager) D-Bus service  when activating and saves the returned cookie on the Method instance. For [`keep.running`](#keep-running-mode) mode uses flag 4 ("Inhibit suspending the session or computer"), and in [`keep.presenting`](#keep-presenting-mode) mode uses the flag 8 ("Inhibit the session being marked as idle"). To deactivate the mode, calls the [Uninhibit](https://lira.no-ip.org:8443/doc/gnome-session/dbus/gnome-session.html#org.gnome.SessionManager.Uninhibit) method of the org.gnome.SessionManager with the cookie.
+- **Multiprocess safe?**: Yes
+- **What if the process holding the lock dies?**: The lock is automatically removed.
+- **How to check it?**:  You may check the list of inhibitors using the [GetInhibitors](https://lira.no-ip.org:8443/doc/gnome-session/dbus/gnome-session.html#org.gnome.SessionManager.GetInhibitors) method, which gives you list of object paths like `["/org/gnome/SessionManager/Inhibitor20"]`. Then you can use the [GetAppId](https://lira.no-ip.org:8443/doc/gnome-session/dbus/gnome-session.html#org.gnome.SessionManager.Inhibitor.GetAppId), [GetFlags](https://lira.no-ip.org:8443/doc/gnome-session/dbus/gnome-session.html#org.gnome.SessionManager.Inhibitor.GetFlags) and [GetReason](https://lira.no-ip.org:8443/doc/gnome-session/dbus/gnome-session.html#org.gnome.SessionManager.Inhibitor.GetReason) methods on the [org.gnome.SessionManager.Inhibitor](https://lira.no-ip.org:8443/doc/gnome-session/dbus/gnome-session.html#org.gnome.SessionManager.Inhibitor) interface of the listed objects on the org.gnome.SessionManager service to translate that into something meaningful. A good tool for this is [D-Spy](https://apps.gnome.org/Dspy/). Alternatively, you could monitor your inhibit call with [`dbus-monitor`](https://dbus.freedesktop.org/doc/dbus-monitor.1.html).
+- **Requirements**: D-Bus, GNOME Desktop Environment with gnome-session running. The exact version of required GNOME is unknown, but this should work from GNOME 2.24 ([2008-09-23](https://gitlab.gnome.org/GNOME/gnome-session/-/tags/GNOME_SESSION_2_24_0)) onwards. See [version history of org.gnome.SessionManager.xml](https://gitlab.gnome.org/GNOME/gnome-session/-/commits/main/gnome-session/org.gnome.SessionManager.xml). At least [this](https://fedoraproject.org/wiki/Desktop/Whiteboards/InhibitApis) and [this](https://bugzilla.redhat.com/show_bug.cgi?id=529287#c3) mention GNOME 2.24.
+- **Tested on**:  Ubuntu 22.04.3 LTS with GNOME 42.9 ([PR #138](https://github.com/fohrloop/wakepy/pull/138) by [fohrloop](https://github.com/fohrloop/)).
+
+````{admonition} May slow down system if called repeatedly
+:class: info
+
+If used thousands of times really fast, may slow down system. See: [wakepy/#277](https://github.com/fohrloop/wakepy/issues/277)
+````
+
+
+(windows-stes)=
+## SetThreadExecutionState
 
 ````{admonition} Windows will not lock the screen automatically if Screen Saver settings do not require it
 :class: warning
 
 Since this method prevents sleep, screen can be only locked automatically if a screen saver is enabled and it set to ask for password. See [this](#checking-if-windows-will-lock-screen-automatically) for details.
 
 ````
 
 - **Name**: `SetThreadExecutionState`
+- **Modes**: [`keep.running`](#keep-running-mode), [`keep.presenting`](#keep-presenting-mode)
 - **Introduced in**: wakepy 0.1.0
-- **How it works**: It calls the [SetThreadExecutionState](https://learn.microsoft.com/en-us/windows/win32/api/winbase/nf-winbase-setthreadexecutionstate) function from the Kernel32.dll with ES_CONTINUOUS and ES_SYSTEM_REQUIRED flags when activating, and with ES_CONTINUOUS when deactivating. Note that currently it is not possible to use two wakepy modes using SetThreadExecutionState at the same time in the same thread! (See: [Issue 167](https://github.com/fohrloop/wakepy/issues/167))
+- **How it works**: It calls the [SetThreadExecutionState](https://learn.microsoft.com/en-us/windows/win32/api/winbase/nf-winbase-setthreadexecutionstate) function from the Kernel32.dll with ES_CONTINUOUS and ES_SYSTEM_REQUIRED flags when activating [`keep.running`](#keep-running-mode) mode, and additionally ES_DISPLAY_REQUIRED flag when activating [`keep.presenting`](#keep-presenting-mode) mode. Uses the  ES_CONTINUOUS flag for deactivating. Note that currently it is not possible to use two wakepy modes using SetThreadExecutionState at the same time in the same thread! (See: [Issue 167](https://github.com/fohrloop/wakepy/issues/167))
 - **Multiprocess safe?**: Yes
 - **What if the process holding the lock dies?**: The lock is automatically removed.
 - **How to check it?**: Run `powercfg /requests` in an elevated cmd or Powershell.
 - **Requirements**: Windows XP or higher (client), Windows Server 2003 or higher (server), as mentioned [here](https://learn.microsoft.com/en-us/windows/win32/api/winbase/nf-winbase-setthreadexecutionstate).
 - **Tested on**:  Windows 10 Pro version 22H2 build 19045.332 with and without Screen Saver + ScreenSaverIsSecure set in settings, Windows 10 Enterprise version 22H2 build 19045.3803 with Group Policies enforcing ScreenSaverIsSecure ([Issue #169](https://github.com/fohrloop/wakepy/issues/169) by [fohrloop](https://github.com/fohrloop/)).
 
 
@@ -97,77 +121,10 @@
 result = ctypes.windll.user32.SystemParametersInfoW(SPI_GETSCREENSAVETIMEOUT, 0, pvparam, 0)
 print('SPI_GETSCREENSAVETIMEOUT', retval.value)
 ```
 
 
 ````
 
-(keep-running-macos-caffeinate)=
-### caffeinate
-
-- **Name**: `caffeinate`
-- **Introduced in**: wakepy 0.3.0
-- **How it works**: It calls the `caffeinate` command. See docs at [ss64.com](https://ss64.com/mac/caffeinate.html) or at archives from [developer.apple.com](https://web.archive.org/web/20140604153141/https://developer.apple.com/library/mac/documentation/Darwin/Reference/ManPages/man8/caffeinate.8.html)
-- **Multiprocess safe?**: Yes
-- **What if the process holding the lock dies?**: The lock is automatically removed.
-- **How to check it?**: You should be able to see a process with a command `/bin/bash caffeinate` or similar associated with it using a task manager.
-- **Requirements**: Mac OS X 10.8 Mountain Lion (July 2012) or newer.
-
-
-## keep.presenting
-
-(keep-presenting-org-gnome-sessionmanager)=
-### org.gnome.SessionManager
-
-- **Name**: `org.gnome.SessionManager`
-- **Introduced in**: wakepy 0.8.0
-- **How it works**: Exactly the same as the [keep.running](#keep-running-org-gnome-sessionmanager) using org.gnome.SessionManager, but using the flag 8 ("Inhibit the session being marked as idle").
-- **Multiprocess safe?**: Yes
-- **What if the process holding the lock dies?**: The lock is automatically removed.
-- **How to check it?**: Similarly as checking [keep.running](#keep-running-org-gnome-sessionmanager) using org.gnome.SessionManager.
-- **Requirements**: Same as [keep.running](#keep-running-org-gnome-sessionmanager) using org.gnome.SessionManager.
-- **Tested on**:  Ubuntu 22.04.3 LTS with GNOME 42.9 ([PR #138](https://github.com/fohrloop/wakepy/pull/138) by [fohrloop](https://github.com/fohrloop/)).
-
-````{admonition} May slow down system if called repeatedly
-:class: warning
-
-If used hundreds or thousands of times, may slow down system. See: [wakepy/#277](https://github.com/fohrloop/wakepy/issues/277)
-````
-
-(keep-presenting-org-freedesktop-screensaver)=
-### org.freedesktop.ScreenSaver
-- **Name**: `org.freedesktop.ScreenSaver`
-- **Introduced in**: wakepy 0.6.0
-- **How it works**: Uses the Inhibit method of [org.freedesktop.ScreenSaver](https://people.freedesktop.org/~hadess/idle-inhibition-spec/re01.html) D-Bus service when activating and saves the returned cookie on the Method instance. Uses the org.freedesktop.ScreenSaver.UnInhibit method with the cookie when deactivating. The org.freedesktop.ScreenSaver can only be used to prevent idle; that is why there is no "keep.running" mode counterpart.
-- **Multiprocess safe?**: Yes
-- **What if the process holding the lock dies?**: The lock is automatically removed.
-- **How to check it?**:  The org.freedesktop.ScreenSaver does not expose a method for listing the inhibitors, but you could monitor your inhibit call with [`dbus-monitor`](https://dbus.freedesktop.org/doc/dbus-monitor.1.html).
-- **Requirements**: D-Bus, and a [freedesktop.org compliant desktop environment](https://www.freedesktop.org/wiki/Desktops/), which should implement the org.freedesktop.ScreenSaver.Inhibit method.
-- **Tested on**:  Ubuntu 22.04 with GNOME 42.9 ([wakepy/#171](https://github.com/fohrloop/wakepy/pull/171)) and openSUSE 15.5 with KDE Plasma 5.27.9 ([wakepy/#310](https://github.com/fohrloop/wakepy/issues/310#issuecomment-2135512139)) by [fohrloop](https://github.com/fohrloop/).
-
-(keep-presenting-windows-stes)=
-### SetThreadExecutionState
 
-- **Name**: `SetThreadExecutionState`
-- **Introduced in**: wakepy 0.1.0
-- **How it works**: Exactly the same as the [keep.running](keep-running-windows-stes), but using ES_CONTINUOUS, ES_SYSTEM_REQUIRED *and* ES_DISPLAY_REQUIRED flags when activating.
-- **Multiprocess safe?**: Yes
-- **What if the process holding the lock dies?**: The lock is automatically removed.
-- **How to check it?**: Like the [keep.running](keep-running-windows-stes)
-- **Requirements**: Same as for the [keep.running](keep-running-windows-stes) using SetThreadExecutionState.
-- **Tested on**:  Windows 10 Pro version 22H2 build 19045.332 with and without Screen Saver + ScreenSaverIsSecure set in settings, Windows 10 Enterprise version 22H2 build 19045.3803 with Group Policies enforcing ScreenSaverIsSecure ([Issue #169](https://github.com/fohrloop/wakepy/issues/169) by [fohrloop](https://github.com/fohrloop/)).
 
 
-
-
-
-(keep-presenting-macos-caffeinate)=
-### caffeinate
-
-- **Name**: `caffeinate`
-- **Introduced in**: wakepy 0.3.0
-- **How it works**: It calls the `caffeinate` command with `-d` flag ("Create an assertion to prevent the display from sleeping."). See docs at [ss64.com](https://ss64.com/mac/caffeinate.html) or at archives from [developer.apple.com](https://web.archive.org/web/20140604153141/https://developer.apple.com/library/mac/documentation/Darwin/Reference/ManPages/man8/caffeinate.8.html)
-- **Multiprocess safe?**: Yes
-- **What if the process holding the lock dies?**: The lock is automatically removed.
-- **How to check it?**: You should be able to see a process with a command `/bin/bash caffeinate -d` or similar associated with it using a task manager.
-- **Requirements**: Mac OS X 10.8 Mountain Lion (July 2012) or newer.
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `wakepy-0.9.0/docs/source/migration.md` & `wakepy-0.9.0.post1/docs/source/migration.md`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/docs/source/modes.md` & `wakepy-0.9.0.post1/docs/source/modes.md`

 * *Files 14% similar despite different names*

```diff
@@ -11,78 +11,86 @@
 
 [^win-slock]: Depending on system settings, it is possible that Windows will not automatically lock the system, because Windows will lock the screen either when (1) returning from suspend (which is now inhibited) or (2) when returning from Screen Saver, *if ScreenSaverIsSecure is set or enforced by a Group Policy (GPO)*.  See: [wakepy/#169](https://github.com/fohrloop/wakepy/issues/169)
 
 ```{note}
 The table above only considers the *automatic* actions (go to sleep, start screenlock, start screensaver), which are based on the *idle timer*; It is still possible to put system to sleep by selecting Suspend/Sleep from a menu, closing the laptop lid or pressing a power key, for example. It is also possible to manually lock the session/screen or start screensaver.
 ```
 
-
 (keep-running-mode)=
 ## keep.running
 
-While `keep.running` mode is activated, the system may not automatically go to sleep (or
-suspend) meaning that programs will continue running and can use CPU.
+While `keep.running` mode is activated, the system may not automatically go to sleep (or suspend) meaning that programs will continue running and can use CPU.
 
+**Python example**
+```{code-block} python
+from wakepy import keep
+
+with keep.running():
+    # Do something that takes a long time. The system may start screensaver
+    # / screenlock or blank the screen, but CPU will keep running.
+```
 
-| Platform | DE    | Method                                                             |
-| -------- | ----- | ------------------------------------------------------------------ |
-| Linux    | GNOME | [org.gnome.SessionManager](#keep-running-org-gnome-sessionmanager) |
-| MacOS    | *     | [caffeinate](#keep-running-macos-caffeinate)                       |
-| Windows  | *     | [SetThreadExecutionState](#keep-running-windows-stes)              |
+```{admonition} See also
+:class: seealso
 
+See the [User Guide](#user-guide) and the API Reference for {func}`keep.running() <wakepy.keep.running>` for more details.
+```
+
+**CLI**
+```{code-block}
+wakepy
+```
 
-Does keep.running prevent manually putting system to sleep?
-: Only the  automatical, idle timer timeout based sleep / suspend is prevented; Will not
-prevent user manually entering sleep from a menu, by closing a laptop lid or by pressing
-a power button, for example.
 
 Can I lock my computer after entered `keep.running` mode?
 : Yes, and you probably should, if you're not near your computer. The program will
 continue execution regardless of the lock.
 
-What about automatical lockscreen / screensaver?
+What about automatical lockscreen / screensaver in `keep.running` mode??
 : The system may still automatically log out user, enable lockscreen or turn off the
-display. Automatic lock screen is not guaranteed, but it is  not prevented in any way.
-
-What happens id the process holding the lock dies?
-: The lock is automatically removed. There are no methods in keep.running mode which for
-example would perform system-wide configuration changes or anything which would need
-manual reversal.
-
-
+display. Automatic lock screen is not guaranteed, but it is  not prevented in any way. Most systems are configured to automatically lock the session after a timeout. One exception is Windows which will lock the screen only either when (1) returning from suspend (which is now inhibited) or (2) when returning from Screen Saver, *if ScreenSaverIsSecure is set or enforced by a Group Policy (GPO)*.  See: [wakepy/#169](https://github.com/fohrloop/wakepy/issues/169)
 
 (keep-presenting-mode)=
 ## keep.presenting
 
-While `keep.presenting` mode is activated, the system may not automatically go to sleep (or
-suspend) meaning that programs will continue running and can use CPU. In addition to
-that, automatic start of screensaver & screenlock are prevented, meaning that you can
+While `keep.presenting` mode is activated, the system may not automatically go to sleep (or suspend) meaning that programs will continue running and can use CPU. In addition to that, automatic start of screensaver & screenlock are prevented, meaning that you can
 show content in the `keep.presenting` mode.
 
+**Python example**
+```{code-block} python
+from wakepy import keep
+
+with keep.presenting():
+    # Do something that takes a long time and requires the screen to be awake
+```
+
+```{admonition} See also
+:class: seealso
+
+See the [User Guide](#user-guide) and the API Reference for {func}`keep.presenting() <wakepy.keep.presenting>` for more details.
+```
+
+**CLI**
+```{code-block}
+wakepy -p
+```
+
 
-| Platform | DE              | Method                                                                      |
-| -------- | --------------- | --------------------------------------------------------------------------- |
-| Linux    | GNOME           | [org.gnome.SessionManager](#keep-presenting-org-gnome-sessionmanager)       |
-| Linux    | GNOME + others? | [org.freedesktop.ScreenSaver](#keep-presenting-org-freedesktop-screensaver) |
-| MacOS    | *               | [caffeinate](#keep-presenting-macos-caffeinate)                             |
-| Windows  | *               | [SetThreadExecutionState](#keep-presenting-windows-stes)                    |
-
-Does keep.presenting prevent manually putting system to sleep?
-: Only the  automatical, idle timer timeout based sleep / suspend is prevented; Will not
-prevent user manually entering sleep from a menu, by closing a laptop lid or by pressing
-a power button, for example.
 
-Can I still manually start lockscreen / screensaver?
+Can I manually start lockscreen / screensaver in `keep.presenting` mode?
 : Yes. Only the idle timer based screensaver / lockscreen is prevented. Note that
 manually entering screensaver does not deactivate the mode.
 
 
+
+## Wakepy Modes FAQ
+
 What happens id the process holding the lock dies?
-: The lock is automatically removed. There are no methods in keep.presenting mode which for
-example would perform system-wide configuration changes or anything which would need
-manual reversal.
+: The lock is automatically removed. Wakepy always leaves the system to a clean state, and does not do any kind of configuration changes or anything which would need manual reversal if the process is killed abruptly.
+
 
+Does wakepy prevent manually putting system to sleep?
+: Only the  automatical, idle timer timeout based sleep / suspend is prevented; Wakepy will not prevent user manually entering sleep from a menu, by closing a laptop lid or by pressing a power button, for example.
 
-## General questions
-**What if the process holding the lock dies?**: The lock is automatically removed.
 
-**How to use wakepy in tests / CI**: One problem with tests and/or CI systems is that many times the environment is different, and preventing system going to sleep works differently there. To fake a successful inhibit lock in tests, you may set an environment variable: [`WAKEPY_FAKE_SUCCESS`](#WAKEPY_FAKE_SUCCESS) to a truthy value like `1`.
+How to use wakepy in tests / CI
+: One problem with tests and/or CI systems is that many times the environment is different, and preventing system going to sleep works differently there. To fake a successful inhibit lock in tests, you may set an environment variable: [`WAKEPY_FAKE_SUCCESS`](#WAKEPY_FAKE_SUCCESS) to a truthy value like `1`.
```

### Comparing `wakepy-0.9.0/docs/source/test-manually.md` & `wakepy-0.9.0.post1/docs/source/test-manually.md`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/docs/source/tests-and-ci.md` & `wakepy-0.9.0.post1/docs/source/tests-and-ci.md`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/docs/source/user-guide.md` & `wakepy-0.9.0.post1/docs/source/user-guide.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # User Guide
 
-Wakepy main Python API is are the wakepy [Modes](#wakepy-modes), which are states that are activated and deactivated and which keep your system awake. The method for activating the mode depends on your platform (among other things) and is determined by the used [Method](#wakepy-methods).  For example [keep.presenting](#keep-presenting-mode) mode is implemented by [org.gnome.SessionManager](#keep-presenting-org-gnome-sessionmanager) for Linux with GNOME DE, [SetThreadExecutionState](#keep-presenting-windows-stes) for Windows and [caffeinate](#keep-presenting-macos-caffeinate) for MacOS. In most cases, wakepy does nothing but calls an executable (caffeinate), a DLL function call (SetThreadExecutionState) or a D-Bus method (org.gnome.SessionManager). Wakepy helps in this by providing a coherent API which should just work™ on any system. Or, at least that is the vision of wakepy.
+Wakepy main Python API is are the wakepy [Modes](#wakepy-modes), which are states that are activated and deactivated and which keep your system awake. The method for activating the mode depends on your platform (among other things) and is determined by the used [Method](#wakepy-methods).  For example [keep.presenting](#keep-presenting-mode) mode is implemented by [org.gnome.SessionManager](#org-gnome-sessionmanager) for Linux with GNOME DE, [SetThreadExecutionState](#windows-stes) for Windows and [caffeinate](#macos-caffeinate) for MacOS. In most cases, wakepy does nothing but calls an executable (caffeinate), a DLL function call (SetThreadExecutionState) or a D-Bus method (org.gnome.SessionManager). Wakepy helps in this by providing a coherent API which should just work™ on any system. Or, at least that is the vision of wakepy.
 
 
 ## Entering a wakepy.Mode
 
 The wakepy modes are implemented as context managers of type {class}`wakepy.Mode`. The available convenience wrappers for creating a Mode are {func}`keep.running() <wakepy.keep.running>` and {func}`keep.presenting() <wakepy.keep.presenting>`. These are used with the `with` statement:
 
 ```{code-block} python
```

### Comparing `wakepy-0.9.0/docs/source/wakepy-mode-lifecycle.md` & `wakepy-0.9.0.post1/docs/source/wakepy-mode-lifecycle.md`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/pyproject.toml` & `wakepy-0.9.0.post1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
+    "Programming Language :: Python :: 3.13",
     "Topic :: Utilities",
 ]
 
 
 [project.urls]
 Homepage = "https://github.com/fohrloop/wakepy"
 "Source Code" = "https://github.com/fohrloop/wakepy"
```

### Comparing `wakepy-0.9.0/requirements/requirements-test.txt` & `wakepy-0.9.0.post1/requirements/requirements-test.txt`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/src/wakepy/__init__.py` & `wakepy-0.9.0.post1/src/wakepy/__init__.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/src/wakepy/__main__.py` & `wakepy-0.9.0.post1/src/wakepy/__main__.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/src/wakepy/core/__init__.py` & `wakepy-0.9.0.post1/src/wakepy/core/__init__.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/src/wakepy/core/activationresult.py` & `wakepy-0.9.0.post1/src/wakepy/core/activationresult.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/src/wakepy/core/constants.py` & `wakepy-0.9.0.post1/src/wakepy/core/constants.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/src/wakepy/core/dbus.py` & `wakepy-0.9.0.post1/src/wakepy/core/dbus.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/src/wakepy/core/heartbeat.py` & `wakepy-0.9.0.post1/src/wakepy/core/heartbeat.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/src/wakepy/core/method.py` & `wakepy-0.9.0.post1/src/wakepy/core/method.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/src/wakepy/core/mode.py` & `wakepy-0.9.0.post1/src/wakepy/core/mode.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/src/wakepy/core/platform.py` & `wakepy-0.9.0.post1/src/wakepy/core/platform.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/src/wakepy/core/prioritization.py` & `wakepy-0.9.0.post1/src/wakepy/core/prioritization.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/src/wakepy/core/registry.py` & `wakepy-0.9.0.post1/src/wakepy/core/registry.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/src/wakepy/core/strenum.py` & `wakepy-0.9.0.post1/src/wakepy/core/strenum.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/src/wakepy/dbus_adapters/jeepney.py` & `wakepy-0.9.0.post1/src/wakepy/dbus_adapters/jeepney.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/src/wakepy/methods/__init__.py` & `wakepy-0.9.0.post1/src/wakepy/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/src/wakepy/methods/_testing.py` & `wakepy-0.9.0.post1/src/wakepy/methods/_testing.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/src/wakepy/methods/freedesktop.py` & `wakepy-0.9.0.post1/src/wakepy/methods/freedesktop.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/src/wakepy/methods/gnome.py` & `wakepy-0.9.0.post1/src/wakepy/methods/gnome.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/src/wakepy/methods/macos.py` & `wakepy-0.9.0.post1/src/wakepy/methods/macos.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/src/wakepy/methods/windows.py` & `wakepy-0.9.0.post1/src/wakepy/methods/windows.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/src/wakepy/modes/keep.py` & `wakepy-0.9.0.post1/src/wakepy/modes/keep.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     omit: Optional[StrCollection] = None,
     methods_priority: Optional[MethodsPriorityOrder] = None,
     on_fail: OnFail = "error",
     dbus_adapter: Type[DBusAdapter] | DBusAdapterTypeSeq | None = None,
 ) -> Mode:
     """Create a wakepy mode (a context manager) for keeping programs running.
 
-    :ref:`Documentation of keep.running mode. <keep-running-mode>`
+    ➡️ :ref:`Documentation of keep.running mode. <keep-running-mode>` ⬅️
 
     Parameters
     ----------
     methods: list, tuple or set of str
         The names of Methods to select from the keep.running mode; a
         "whitelist" filter. Means "use these and only these Methods". Any
         Methods in `methods` but not in the keep.running mode will raise a
@@ -93,15 +93,15 @@
     methods_priority: Optional[MethodsPriorityOrder] = None,
     on_fail: OnFail = "error",
     dbus_adapter: Type[DBusAdapter] | DBusAdapterTypeSeq | None = None,
 ) -> Mode:
     """Create a wakepy mode (a context manager) for keeping a system running
     and showing content.
 
-    :ref:`Documentation of keep.presenting mode. <keep-presenting-mode>`
+    ➡️ :ref:`Documentation of keep.presenting mode. <keep-presenting-mode>` ⬅️
 
     Parameters
     ----------
     methods: list, tuple or set of str
         The names of Methods to select from the keep.presenting mode; a
         "whitelist" filter. Means "use these and only these Methods". Any
         Methods in `methods` but not in the keep.presenting mode will raise a
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `wakepy-0.9.0/src/wakepy.egg-info/SOURCES.txt` & `wakepy-0.9.0.post1/src/wakepy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/tasks.py` & `wakepy-0.9.0.post1/tasks.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/tests/conftest.py` & `wakepy-0.9.0.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/tests/integration/conftest.py` & `wakepy-0.9.0.post1/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/tests/integration/dbus_service.py` & `wakepy-0.9.0.post1/tests/integration/dbus_service.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/tests/integration/test_dbus_adapters.py` & `wakepy-0.9.0.post1/tests/integration/test_dbus_adapters.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/tests/tox_build_wakepy.py` & `wakepy-0.9.0.post1/tests/tox_build_wakepy.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/tests/unit/conftest.py` & `wakepy-0.9.0.post1/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/tests/unit/test__init__.py` & `wakepy-0.9.0.post1/tests/unit/test__init__.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/tests/unit/test_core/conftest.py` & `wakepy-0.9.0.post1/tests/unit/test_core/conftest.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/tests/unit/test_core/test_activationresult.py` & `wakepy-0.9.0.post1/tests/unit/test_core/test_activationresult.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/tests/unit/test_core/test_calls.py` & `wakepy-0.9.0.post1/tests/unit/test_core/test_calls.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/tests/unit/test_core/test_dbus.py` & `wakepy-0.9.0.post1/tests/unit/test_core/test_dbus.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/tests/unit/test_core/test_method/test_activation.py` & `wakepy-0.9.0.post1/tests/unit/test_core/test_method/test_activation.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/tests/unit/test_core/test_method/test_method.py` & `wakepy-0.9.0.post1/tests/unit/test_core/test_method/test_method.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/tests/unit/test_core/test_mode.py` & `wakepy-0.9.0.post1/tests/unit/test_core/test_mode.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/tests/unit/test_core/test_platform.py` & `wakepy-0.9.0.post1/tests/unit/test_core/test_platform.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/tests/unit/test_core/test_prioritization.py` & `wakepy-0.9.0.post1/tests/unit/test_core/test_prioritization.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/tests/unit/test_core/test_registry.py` & `wakepy-0.9.0.post1/tests/unit/test_core/test_registry.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/tests/unit/test_core/test_strenum.py` & `wakepy-0.9.0.post1/tests/unit/test_core/test_strenum.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/tests/unit/test_core/testmethods.py` & `wakepy-0.9.0.post1/tests/unit/test_core/testmethods.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/tests/unit/test_main.py` & `wakepy-0.9.0.post1/tests/unit/test_main.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/tests/unit/test_methods/test_freedesktop.py` & `wakepy-0.9.0.post1/tests/unit/test_methods/test_freedesktop.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/tests/unit/test_methods/test_gnome.py` & `wakepy-0.9.0.post1/tests/unit/test_methods/test_gnome.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/tests/unit/test_methods/test_macos.py` & `wakepy-0.9.0.post1/tests/unit/test_methods/test_macos.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/tests/unit/test_methods/test_windows.py` & `wakepy-0.9.0.post1/tests/unit/test_methods/test_windows.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/tests/unit/test_modes.py` & `wakepy-0.9.0.post1/tests/unit/test_modes.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/tox.ini` & `wakepy-0.9.0.post1/tox.ini`

 * *Files identical despite different names*

### Comparing `wakepy-0.9.0/toxfile.py` & `wakepy-0.9.0.post1/toxfile.py`

 * *Files identical despite different names*

