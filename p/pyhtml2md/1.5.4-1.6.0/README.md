# Comparing `tmp/pyhtml2md-1.5.4.tar.gz` & `tmp/pyhtml2md-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhtml2md-1.5.4.tar", last modified: Thu Apr 18 07:59:18 2024, max compression
+gzip compressed data, was "pyhtml2md-1.6.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `pyhtml2md-1.5.4.tar` & `pyhtml2md-1.6.0.tar`

### file list

```diff
@@ -1,87 +1,380 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:59:18.721184 pyhtml2md-1.5.4/
--rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-04-18 07:59:18.721184 pyhtml2md-1.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:59:18.709184 pyhtml2md-1.5.4/include/
--rw-r--r--   0 runner    (1001) docker     (127)    16467 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/include/html2md.h
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/include/table.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:59:18.721184 pyhtml2md-1.5.4/pyhtml2md.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-04-18 07:59:18.000000 pyhtml2md-1.5.4/pyhtml2md.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-18 07:59:18.000000 pyhtml2md-1.5.4/pyhtml2md.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 07:59:18.000000 pyhtml2md-1.5.4/pyhtml2md.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 07:59:18.000000 pyhtml2md-1.5.4/pyhtml2md.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-18 07:59:18.000000 pyhtml2md-1.5.4/pyhtml2md.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-18 07:59:18.000000 pyhtml2md-1.5.4/pyhtml2md.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:59:18.709184 pyhtml2md-1.5.4/python/
--rw-r--r--   0 runner    (1001) docker     (127)     5173 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/bindings.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:59:18.709184 pyhtml2md-1.5.4/python/pybind11/
--rw-r--r--   0 runner    (1001) docker     (127)    14018 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:59:18.705184 pyhtml2md-1.5.4/python/pybind11/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:59:18.717184 pyhtml2md-1.5.4/python/pybind11/include/pybind11/
--rw-r--r--   0 runner    (1001) docker     (127)    24334 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner    (1001) docker     (127)     7778 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner    (1001) docker     (127)    71139 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner    (1001) docker     (127)     8458 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:59:18.717184 pyhtml2md-1.5.4/python/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner    (1001) docker     (127)    28563 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner    (1001) docker     (127)    53818 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner    (1001) docker     (127)    17858 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner    (1001) docker     (127)    29071 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner    (1001) docker     (127)    49998 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/detail/typeid.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:59:18.717184 pyhtml2md-1.5.4/python/pybind11/include/pybind11/eigen/
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/eigen/common.h
--rw-r--r--   0 runner    (1001) docker     (127)    32135 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/eigen/matrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    18490 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/eigen/tensor.h
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner    (1001) docker     (127)    13459 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner    (1001) docker     (127)     4731 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/gil.h
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/gil_safe_call_once.h
--rw-r--r--   0 runner    (1001) docker     (127)     8862 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner    (1001) docker     (127)    84243 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 runner    (1001) docker     (127)     9103 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner    (1001) docker     (127)   129569 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner    (1001) docker     (127)    98953 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:59:18.717184 pyhtml2md-1.5.4/python/pybind11/include/pybind11/stl/
--rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 runner    (1001) docker     (127)    15532 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner    (1001) docker     (127)    28463 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/stl_bind.h
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/type_caster_pyobject_ptr.h
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/include/pybind11/typing.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:59:18.721184 pyhtml2md-1.5.4/python/pybind11/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 runner    (1001) docker     (127)    12183 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/tools/FindPythonLibsNew.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/tools/JoinPaths.cmake
--rwxr-xr-x   0 runner    (1001) docker     (127)     1423 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/tools/check-style.sh
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/tools/codespell_ignore_lines_from_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/tools/libsize.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2090 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/tools/make_changelog.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/tools/pybind11.pc.in
--rw-r--r--   0 runner    (1001) docker     (127)    15032 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     7101 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (127)    10970 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     8569 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/tools/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/tools/setup_global.py.in
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/python/pybind11/tools/setup_main.py.in
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 07:59:18.721184 pyhtml2md-1.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5889 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:59:18.721184 pyhtml2md-1.5.4/src/
--rw-r--r--   0 runner    (1001) docker     (127)    23244 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/src/html2md.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/src/table.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:59:18.721184 pyhtml2md-1.5.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/tests/test_advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-18 07:59:12.000000 pyhtml2md-1.5.4/tests/test_basic.py
+-rw-r--r--   0        0        0     5421 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/.clang-format
+-rw-r--r--   0        0        0       31 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      557 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      122 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0        0        0      614 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      473 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0     2180 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0      607 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/.github/workflows/website.yml
+-rw-r--r--   0        0        0     1356 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/.github/workflows/wheels.yml
+-rw-r--r--   0        0        0      146 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/.gitignore
+-rw-r--r--   0        0        0      197 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/.gitmodules
+-rw-r--r--   0        0        0     2591 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0     4454 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/CMakeLists.txt
+-rw-r--r--   0        0        0       76 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1069 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/COPYING
+-rw-r--r--   0        0        0      205 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/MANIFEST.in
+-rw-r--r--   0        0        0     5588 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/README.md
+-rw-r--r--   0        0        0      368 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/SECURITY.md
+-rw-r--r--   0        0        0     4373 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/cli/main.cpp
+-rw-r--r--   0        0        0      407 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/cmake/Doc.cmake
+-rw-r--r--   0        0        0     3882 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/cmake/Packaging.cmake
+-rw-r--r--   0        0        0     1624 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/docs/Doxyfile
+-rw-r--r--   0        0        0       25 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/docs/doxygen-awesome-css/.gitignore
+-rw-r--r--   0        0        0     1065 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/docs/doxygen-awesome-css/LICENSE
+-rw-r--r--   0        0        0     8469 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/docs/doxygen-awesome-css/doxygen-awesome-darkmode-toggle.js
+-rw-r--r--   0        0        0     4035 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/docs/doxygen-awesome-css/doxygen-awesome-fragment-copy-button.js
+-rw-r--r--   0        0        0     3170 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/docs/doxygen-awesome-css/doxygen-awesome-interactive-toc.js
+-rw-r--r--   0        0        0     2440 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/docs/doxygen-awesome-css/doxygen-awesome-paragraph-link.js
+-rw-r--r--   0        0        0     1467 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/docs/doxygen-awesome-css/doxygen-awesome-sidebar-only-darkmode-toggle.css
+-rw-r--r--   0        0        0     3236 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/docs/doxygen-awesome-css/doxygen-awesome-sidebar-only.css
+-rw-r--r--   0        0        0    60066 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/docs/doxygen-awesome-css/doxygen-awesome.css
+-rw-r--r--   0        0        0     2701 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/docs/doxygen-awesome-css/doxygen-custom/custom.css
+-rw-r--r--   0        0        0     5108 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/docs/doxygen-awesome-css/doxygen-custom/header.html
+-rw-r--r--   0        0        0     4684 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/docs/index.md
+-rw-r--r--   0        0        0      314 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/html2md.pc.in
+-rw-r--r--   0        0        0      131 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/html2mdConfig.cmake.in
+-rw-r--r--   0        0        0    16872 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/include/html2md.h
+-rw-r--r--   0        0        0      252 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/include/table.h
+-rw-r--r--   0        0        0      796 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/js/bindings.cpp
+-rw-r--r--   0        0        0     2160 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     5173 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/README.md
+-rw-r--r--   0        0        0     1524 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/bindings.cpp
+-rw-r--r--   0        0        0     1271 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/.appveyor.yml
+-rw-r--r--   0        0        0      996 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/.clang-format
+-rw-r--r--   0        0        0     2605 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/.clang-tidy
+-rw-r--r--   0        0        0     2196 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/.cmake-format.yaml
+-rw-r--r--   0        0        0     1308 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/.codespell-ignore-lines
+-rw-r--r--   0        0        0       43 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/.git
+-rw-r--r--   0        0        0       18 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/.gitattributes
+-rw-r--r--   0        0        0      182 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/.github/CODEOWNERS
+-rw-r--r--   0        0        0    15285 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2561 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0        0        0      328 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      313 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/.github/dependabot.yml
+-rw-r--r--   0        0        0      116 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/.github/labeler.yml
+-rw-r--r--   0        0        0       50 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/.github/labeler_merged.yml
+-rw-r--r--   0        0        0      668 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      645 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/.github/pull_request_template.md
+-rw-r--r--   0        0        0    35430 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2271 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/.github/workflows/configure.yml
+-rw-r--r--   0        0        0     1491 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/.github/workflows/format.yml
+-rw-r--r--   0        0        0      639 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/.github/workflows/labeler.yml
+-rw-r--r--   0        0        0     2628 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/.github/workflows/pip.yml
+-rw-r--r--   0        0        0     2876 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/.github/workflows/upstream.yml
+-rw-r--r--   0        0        0      502 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/.gitignore
+-rw-r--r--   0        0        0     3647 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      276 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/.readthedocs.yml
+-rw-r--r--   0        0        0    14018 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/CMakeLists.txt
+-rw-r--r--   0        0        0     1684 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/LICENSE
+-rw-r--r--   0        0        0      247 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/MANIFEST.in
+-rw-r--r--   0        0        0     7737 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/README.rst
+-rw-r--r--   0        0        0      688 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/SECURITY.md
+-rw-r--r--   0        0        0      607 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/docs/Doxyfile
+-rw-r--r--   0        0        0     7417 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/docs/Makefile
+-rw-r--r--   0        0        0       37 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/docs/_static/css/custom.css
+-rw-r--r--   0        0        0     3937 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/docs/advanced/cast/chrono.rst
+-rw-r--r--   0        0        0     3429 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/docs/advanced/cast/custom.rst
+-rw-r--r--   0        0        0    14283 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/docs/advanced/cast/eigen.rst
+-rw-r--r--   0        0        0     3889 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/docs/advanced/cast/functional.rst
+-rw-r--r--   0        0        0     1556 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/docs/advanced/cast/index.rst
+-rw-r--r--   0        0        0    12371 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/docs/advanced/cast/overview.rst
+-rw-r--r--   0        0        0     9586 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/docs/advanced/cast/stl.rst
+-rw-r--r--   0        0        0     9119 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/docs/advanced/cast/strings.rst
+-rw-r--r--   0        0        0    47796 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/docs/advanced/classes.rst
+-rw-r--r--   0        0        0     8460 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/docs/advanced/embedding.rst
+-rw-r--r--   0        0        0    17846 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/docs/advanced/exceptions.rst
+-rw-r--r--   0        0        0    26727 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/docs/advanced/functions.rst
+-rw-r--r--   0        0        0    16583 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/docs/advanced/misc.rst
+-rw-r--r--   0        0        0      278 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/docs/advanced/pycpp/index.rst
+-rw-r--r--   0        0        0    17161 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/docs/advanced/pycpp/numpy.rst
+-rw-r--r--   0        0        0     9030 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/docs/advanced/pycpp/object.rst
+-rw-r--r--   0        0        0     5710 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/docs/advanced/pycpp/utilities.rst
+-rw-r--r--   0        0        0     6377 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/docs/advanced/smart_ptrs.rst
+-rw-r--r--   0        0        0     9240 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/docs/basics.rst
+-rw-r--r--   0        0        0     2853 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/docs/benchmark.py
+-rw-r--r--   0        0        0     3168 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/docs/benchmark.rst
+-rw-r--r--   0        0        0   126560 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/docs/changelog.rst
+-rw-r--r--   0        0        0    17090 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/docs/classes.rst
+-rw-r--r--   0        0        0      273 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/docs/cmake/index.rst
+-rw-r--r--   0        0        0    26301 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/docs/compiling.rst
+-rw-r--r--   0        0        0    11574 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/docs/conf.py
+-rw-r--r--   0        0        0    13293 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/docs/faq.rst
+-rw-r--r--   0        0        0      613 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/docs/index.rst
+-rw-r--r--   0        0        0     3277 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/docs/installing.rst
+-rw-r--r--   0        0        0     3079 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/docs/limitations.rst
+-rw-r--r--   0        0        0    61034 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/docs/pybind11-logo.png
+-rw-r--r--   0        0        0    44653 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/docs/pybind11_vs_boost_python1.png
+-rw-r--r--   0        0        0    87708 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/docs/pybind11_vs_boost_python1.svg
+-rw-r--r--   0        0        0    41121 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/docs/pybind11_vs_boost_python2.png
+-rw-r--r--   0        0        0    85853 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/docs/pybind11_vs_boost_python2.svg
+-rw-r--r--   0        0        0     2647 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/docs/reference.rst
+-rw-r--r--   0        0        0     4948 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/docs/release.rst
+-rw-r--r--   0        0        0      149 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/docs/requirements.txt
+-rw-r--r--   0        0        0    25209 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/docs/upgrade.rst
+-rw-r--r--   0        0        0    24334 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/include/pybind11/attr.h
+-rw-r--r--   0        0        0     7778 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0        0        0    71139 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/include/pybind11/cast.h
+-rw-r--r--   0        0        0     8458 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0        0        0      120 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/include/pybind11/common.h
+-rw-r--r--   0        0        0     2096 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/include/pybind11/complex.h
+-rw-r--r--   0        0        0    28563 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0        0        0    53818 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0        0        0     6035 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0        0        0    17858 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0        0        0    29071 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0        0        0    49998 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0        0        0     1625 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/include/pybind11/detail/typeid.h
+-rw-r--r--   0        0        0      378 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/include/pybind11/eigen/common.h
+-rw-r--r--   0        0        0    32135 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/include/pybind11/eigen/matrix.h
+-rw-r--r--   0        0        0    18490 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/include/pybind11/eigen/tensor.h
+-rw-r--r--   0        0        0      316 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0        0        0    13459 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/include/pybind11/embed.h
+-rw-r--r--   0        0        0     4731 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/include/pybind11/eval.h
+-rw-r--r--   0        0        0     5051 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/include/pybind11/functional.h
+-rw-r--r--   0        0        0     8517 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/include/pybind11/gil.h
+-rw-r--r--   0        0        0     3876 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/include/pybind11/gil_safe_call_once.h
+-rw-r--r--   0        0        0     8862 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0        0        0    84243 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0        0        0     9103 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/include/pybind11/operators.h
+-rw-r--r--   0        0        0     2734 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/include/pybind11/options.h
+-rw-r--r--   0        0        0   129569 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0        0        0    98953 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/include/pybind11/pytypes.h
+-rw-r--r--   0        0        0     4185 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0        0        0    15532 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/include/pybind11/stl.h
+-rw-r--r--   0        0        0    28463 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/include/pybind11/stl_bind.h
+-rw-r--r--   0        0        0     1929 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/include/pybind11/type_caster_pyobject_ptr.h
+-rw-r--r--   0        0        0     3600 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/include/pybind11/typing.h
+-rw-r--r--   0        0        0     2746 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/noxfile.py
+-rw-r--r--   0        0        0      429 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/pybind11/__init__.py
+-rw-r--r--   0        0        0     1544 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/pybind11/__main__.py
+-rw-r--r--   0        0        0      233 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/pybind11/_version.py
+-rw-r--r--   0        0        0     1207 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/pybind11/commands.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/pybind11/py.typed
+-rw-r--r--   0        0        0    17504 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/pybind11/setup_helpers.py
+-rw-r--r--   0        0        0     2232 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/pyproject.toml
+-rw-r--r--   0        0        0     1495 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/setup.cfg
+-rw-r--r--   0        0        0     4855 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/setup.py
+-rw-r--r--   0        0        0    21874 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/CMakeLists.txt
+-rw-r--r--   0        0        0     5692 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/conftest.py
+-rw-r--r--   0        0        0    11736 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/constructor_stats.h
+-rw-r--r--   0        0        0     3578 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/cross_module_gil_utils.cpp
+-rw-r--r--   0        0        0     1772 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/cross_module_interleaved_error_already_set.cpp
+-rw-r--r--   0        0        0      396 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/eigen_tensor_avoid_stl_array.cpp
+-rw-r--r--   0        0        0      926 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/env.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/extra_python_package/pytest.ini
+-rw-r--r--   0        0        0     8481 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/extra_python_package/test_files.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/extra_setuptools/pytest.ini
+-rw-r--r--   0        0        0     4153 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/extra_setuptools/test_setuphelper.py
+-rw-r--r--   0        0        0     2847 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/local_bindings.h
+-rw-r--r--   0        0        0     5743 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/object.h
+-rw-r--r--   0        0        0     6256 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/pybind11_cross_module_tests.cpp
+-rw-r--r--   0        0        0     4632 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/pybind11_tests.cpp
+-rw-r--r--   0        0        0     2685 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/pybind11_tests.h
+-rw-r--r--   0        0        0      768 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/pytest.ini
+-rw-r--r--   0        0        0      995 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/requirements.txt
+-rw-r--r--   0        0        0      855 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_async.cpp
+-rw-r--r--   0        0        0      536 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_async.py
+-rw-r--r--   0        0        0    10548 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_buffers.cpp
+-rw-r--r--   0        0        0     7124 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_buffers.py
+-rw-r--r--   0        0        0    15948 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_builtin_casters.cpp
+-rw-r--r--   0        0        0    17243 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_builtin_casters.py
+-rw-r--r--   0        0        0     4100 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_call_policies.cpp
+-rw-r--r--   0        0        0     6549 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_call_policies.py
+-rw-r--r--   0        0        0    10858 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_callbacks.cpp
+-rw-r--r--   0        0        0     6955 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_callbacks.py
+-rw-r--r--   0        0        0     3370 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_chrono.cpp
+-rw-r--r--   0        0        0     5691 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_chrono.py
+-rw-r--r--   0        0        0    24836 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_class.cpp
+-rw-r--r--   0        0        0    15187 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_class.py
+-rw-r--r--   0        0        0     2581 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_cmake_build/CMakeLists.txt
+-rw-r--r--   0        0        0      673 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_cmake_build/embed.cpp
+-rw-r--r--   0        0        0     1171 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+-rw-r--r--   0        0        0     1293 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+-rw-r--r--   0        0        0     1685 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+-rw-r--r--   0        0        0      152 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_cmake_build/main.cpp
+-rw-r--r--   0        0        0     1609 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+-rw-r--r--   0        0        0     1419 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+-rw-r--r--   0        0        0     1624 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+-rw-r--r--   0        0        0      198 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_cmake_build/test.py
+-rw-r--r--   0        0        0     3831 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_const_name.cpp
+-rw-r--r--   0        0        0      593 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_const_name.py
+-rw-r--r--   0        0        0     5846 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_constants_and_functions.cpp
+-rw-r--r--   0        0        0     1551 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_constants_and_functions.py
+-rw-r--r--   0        0        0    26055 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_copy_move.cpp
+-rw-r--r--   0        0        0     4796 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_copy_move.py
+-rw-r--r--   0        0        0     7536 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_custom_type_casters.cpp
+-rw-r--r--   0        0        0     3992 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_custom_type_casters.py
+-rw-r--r--   0        0        0     1259 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_custom_type_setup.cpp
+-rw-r--r--   0        0        0     1091 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_custom_type_setup.py
+-rw-r--r--   0        0        0     4405 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_docstring_options.cpp
+-rw-r--r--   0        0        0     2423 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_docstring_options.py
+-rw-r--r--   0        0        0    19932 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_eigen_matrix.cpp
+-rw-r--r--   0        0        0    29175 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_eigen_matrix.py
+-rw-r--r--   0        0        0      473 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_eigen_tensor.cpp
+-rw-r--r--   0        0        0    10581 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_eigen_tensor.inl
+-rw-r--r--   0        0        0     9414 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_eigen_tensor.py
+-rw-r--r--   0        0        0     1798 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_embed/CMakeLists.txt
+-rw-r--r--   0        0        0     1315 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_embed/catch.cpp
+-rw-r--r--   0        0        0      543 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_embed/external_module.cpp
+-rw-r--r--   0        0        0    17396 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_embed/test_interpreter.cpp
+-rw-r--r--   0        0        0      237 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_embed/test_interpreter.py
+-rw-r--r--   0        0        0      275 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_embed/test_trampoline.py
+-rw-r--r--   0        0        0     5722 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_enum.cpp
+-rw-r--r--   0        0        0     9069 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_enum.py
+-rw-r--r--   0        0        0     3168 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_eval.cpp
+-rw-r--r--   0        0        0     1143 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_eval.py
+-rw-r--r--   0        0        0      119 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_eval_call.py
+-rw-r--r--   0        0        0    13851 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_exceptions.cpp
+-rw-r--r--   0        0        0      397 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_exceptions.h
+-rw-r--r--   0        0        0    14537 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_exceptions.py
+-rw-r--r--   0        0        0    18155 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_factory_constructors.cpp
+-rw-r--r--   0        0        0    16491 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_factory_constructors.py
+-rw-r--r--   0        0        0     5311 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_gil_scoped.cpp
+-rw-r--r--   0        0        0     8507 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_gil_scoped.py
+-rw-r--r--   0        0        0     3960 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_iostream.cpp
+-rw-r--r--   0        0        0     7144 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_iostream.py
+-rw-r--r--   0        0        0    10989 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_kwargs_and_defaults.cpp
+-rw-r--r--   0        0        0    14856 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_kwargs_and_defaults.py
+-rw-r--r--   0        0        0     4401 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_local_bindings.cpp
+-rw-r--r--   0        0        0     8054 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_local_bindings.py
+-rw-r--r--   0        0        0    22202 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_methods_and_attributes.cpp
+-rw-r--r--   0        0        0    18426 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_methods_and_attributes.py
+-rw-r--r--   0        0        0     4121 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_modules.cpp
+-rw-r--r--   0        0        0     3963 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_modules.py
+-rw-r--r--   0        0        0    12305 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_multiple_inheritance.cpp
+-rw-r--r--   0        0        0    11874 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_multiple_inheritance.py
+-rw-r--r--   0        0        0    20907 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_numpy_array.cpp
+-rw-r--r--   0        0        0    23073 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_numpy_array.py
+-rw-r--r--   0        0        0    21517 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_numpy_dtypes.cpp
+-rw-r--r--   0        0        0    14619 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_numpy_dtypes.py
+-rw-r--r--   0        0        0     4487 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_numpy_vectorize.cpp
+-rw-r--r--   0        0        0     9658 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_numpy_vectorize.py
+-rw-r--r--   0        0        0     2777 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_opaque_types.cpp
+-rw-r--r--   0        0        0     1847 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_opaque_types.py
+-rw-r--r--   0        0        0     9132 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_operator_overloading.cpp
+-rw-r--r--   0        0        0     4332 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_operator_overloading.py
+-rw-r--r--   0        0        0     6719 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_pickling.cpp
+-rw-r--r--   0        0        0     2720 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_pickling.py
+-rw-r--r--   0        0        0     1555 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_python_multiple_inheritance.cpp
+-rw-r--r--   0        0        0      859 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_python_multiple_inheritance.py
+-rw-r--r--   0        0        0    32112 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_pytypes.cpp
+-rw-r--r--   0        0        0    25274 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_pytypes.py
+-rw-r--r--   0        0        0    21920 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_sequences_and_iterators.cpp
+-rw-r--r--   0        0        0     8659 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_sequences_and_iterators.py
+-rw-r--r--   0        0        0    19028 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_smart_ptr.cpp
+-rw-r--r--   0        0        0     9530 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_smart_ptr.py
+-rw-r--r--   0        0        0    21576 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_stl.cpp
+-rw-r--r--   0        0        0    12307 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_stl.py
+-rw-r--r--   0        0        0     8697 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_stl_binders.cpp
+-rw-r--r--   0        0        0    11043 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_stl_binders.py
+-rw-r--r--   0        0        0     4617 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_tagbased_polymorphic.cpp
+-rw-r--r--   0        0        0      741 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_tagbased_polymorphic.py
+-rw-r--r--   0        0        0     1855 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_thread.cpp
+-rw-r--r--   0        0        0      826 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_thread.py
+-rw-r--r--   0        0        0     4497 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_type_caster_pyobject_ptr.cpp
+-rw-r--r--   0        0        0     3260 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_type_caster_pyobject_ptr.py
+-rw-r--r--   0        0        0      603 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_union.cpp
+-rw-r--r--   0        0        0      148 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_union.py
+-rw-r--r--   0        0        0      845 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_unnamed_namespace_a.cpp
+-rw-r--r--   0        0        0     1141 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_unnamed_namespace_a.py
+-rw-r--r--   0        0        0      341 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_unnamed_namespace_b.cpp
+-rw-r--r--   0        0        0      143 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_unnamed_namespace_b.py
+-rw-r--r--   0        0        0     1471 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_vector_unique_ptr_member.cpp
+-rw-r--r--   0        0        0      329 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_vector_unique_ptr_member.py
+-rw-r--r--   0        0        0    22991 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_virtual_functions.cpp
+-rw-r--r--   0        0        0    12913 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/test_virtual_functions.py
+-rw-r--r--   0        0        0     3226 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/valgrind-numpy-scipy.supp
+-rw-r--r--   0        0        0     2657 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tests/valgrind-python.supp
+-rw-r--r--   0        0        0     2449 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0        0        0     3105 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0        0        0    12183 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tools/FindPythonLibsNew.cmake
+-rw-r--r--   0        0        0      817 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tools/JoinPaths.cmake
+-rwxr-xr-x   0        0        0     1423 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tools/check-style.sh
+-rw-r--r--   0        0        0      952 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0        0        0     1117 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tools/codespell_ignore_lines_from_errors.py
+-rw-r--r--   0        0        0     1031 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tools/libsize.py
+-rwxr-xr-x   0        0        0     2090 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tools/make_changelog.py
+-rw-r--r--   0        0        0      196 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tools/pybind11.pc.in
+-rw-r--r--   0        0        0    15032 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0        0        0     7101 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0        0        0    10970 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0        0        0     8569 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0        0        0       94 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tools/pyproject.toml
+-rw-r--r--   0        0        0     2104 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tools/setup_global.py.in
+-rw-r--r--   0        0        0     1234 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/python/pybind11/tools/setup_main.py.in
+-rwxr-xr-x   0        0        0      120 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/scripts/clang-format.sh
+-rw-r--r--   0        0        0    23328 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/src/html2md.cpp
+-rw-r--r--   0        0        0     2633 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/src/table.cpp
+-rw-r--r--   0        0        0     1163 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/CMakeLists.txt
+-rw-r--r--   0        0        0      427 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/README.md
+-rw-r--r--   0        0        0     1234 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/blockquote.md
+-rw-r--r--   0        0        0      403 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/breaks.md
+-rw-r--r--   0        0        0     1078 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/code.md
+-rw-r--r--   0        0        0      220 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/comment.html
+-rw-r--r--   0        0        0      439 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/escaping.md
+-rw-r--r--   0        0        0      524 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/formating.md
+-rw-r--r--   0        0        0     1067 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/links.md
+-rw-r--r--   0        0        0      116 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/lists.md
+-rw-r--r--   0        0        0     5938 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/main.cpp
+-rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/.git
+-rw-r--r--   0        0        0      661 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/.gitignore
+-rw-r--r--   0        0        0     1156 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/.travis.yml
+-rw-r--r--   0        0        0    15469 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/CHANGELOG.md
+-rw-r--r--   0        0        0     2044 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/CMakeLists.txt
+-rw-r--r--   0        0        0     1096 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/LICENSE.md
+-rw-r--r--   0        0        0    12768 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/README.md
+-rw-r--r--   0        0        0      560 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/appveyor.yml
+-rw-r--r--   0        0        0       81 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/codecov.yml
+-rw-r--r--   0        0        0      576 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/md2html/CMakeLists.txt
+-rw-r--r--   0        0        0     8313 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/md2html/cmdline.c
+-rw-r--r--   0        0        0     6155 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/md2html/cmdline.h
+-rw-r--r--   0        0        0     1746 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/md2html/md2html.1
+-rw-r--r--   0        0        0    14681 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/md2html/md2html.c
+-rw-r--r--   0        0        0     4351 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/scripts/build_folding_map.py
+-rw-r--r--   0        0        0     1781 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/scripts/build_punct_map.py
+-rw-r--r--   0        0        0     1764 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/scripts/build_symbol_map.py
+-rw-r--r--   0        0        0     1750 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/scripts/build_whitespace_map.py
+-rwxr-xr-x   0        0        0     1488 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/scripts/coverity.sh
+-rwxr-xr-x   0        0        0     2752 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/scripts/run-tests.sh
+-rw-r--r--   0        0        0    82810 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/scripts/unicode/CaseFolding.txt
+-rw-r--r--   0        0        0   259503 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/scripts/unicode/DerivedGeneralCategory.txt
+-rw-r--r--   0        0        0     1679 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/src/CMakeLists.txt
+-rw-r--r--   0        0        0    74111 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/src/entity.c
+-rw-r--r--   0        0        0     1573 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/src/entity.h
+-rw-r--r--   0        0        0    20297 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/src/md4c-html.c
+-rw-r--r--   0        0        0     2651 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/src/md4c-html.h
+-rw-r--r--   0        0        0      379 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/src/md4c-html.pc.in
+-rw-r--r--   0        0        0   253338 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/src/md4c.c
+-rw-r--r--   0        0        0    15931 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/src/md4c.h
+-rw-r--r--   0        0        0      365 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/src/md4c.pc.in
+-rw-r--r--   0        0        0     2791 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/test/LICENSE
+-rwxr-xr-x   0        0        0     1372 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/test/cmark.py
+-rw-r--r--   0        0        0    10519 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/test/coverage.txt
+-rw-r--r--   0        0        0      424 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/test/fuzz-input/commonmark.md
+-rw-r--r--   0        0        0      133 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/test/fuzz-input/gfm.md
+-rw-r--r--   0        0        0       30 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/test/fuzz-input/latex-math.md
+-rw-r--r--   0        0        0       24 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/test/fuzz-input/wiki.md
+-rw-r--r--   0        0        0      820 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/test/fuzzers/fuzz-mdhtml.c
+-rw-r--r--   0        0        0     3740 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/test/heading-auto-identifier.txt
+-rw-r--r--   0        0        0     1136 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/test/latex-math.txt
+-rwxr-xr-x   0        0        0     6508 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/test/normalize.py
+-rwxr-xr-x   0        0        0     2242 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/test/pathological_auto_ident_tests.py
+-rwxr-xr-x   0        0        0     4782 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/test/pathological_tests.py
+-rw-r--r--   0        0        0     1511 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/test/permissive-email-autolinks.txt
+-rw-r--r--   0        0        0     3088 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/test/permissive-url-autolinks.txt
+-rw-r--r--   0        0        0     4049 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/test/permissive-www-autolinks.txt
+-rw-r--r--   0        0        0   204973 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/test/spec.txt
+-rwxr-xr-x   0        0        0     5924 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/test/spec_tests.py
+-rw-r--r--   0        0        0     1677 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/test/strikethrough.txt
+-rw-r--r--   0        0        0     7065 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/test/tables.txt
+-rw-r--r--   0        0        0     3590 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/test/tasklists.txt
+-rw-r--r--   0        0        0     1721 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/test/toc-mark.txt
+-rw-r--r--   0        0        0     2209 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/test/toc.txt
+-rw-r--r--   0        0        0      983 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/test/underline.txt
+-rw-r--r--   0        0        0     5994 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/md4c/test/wiki-links.txt
+-rw-r--r--   0        0        0      755 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/tables.md
+-rw-r--r--   0        0        0      250 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/test_advanced.py
+-rw-r--r--   0        0        0      114 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/tests/test_basic.py
+-rw-r--r--   0        0        0     6230 2022-11-09 12:37:21.000000 pyhtml2md-1.6.0/PKG-INFO
```

### Comparing `pyhtml2md-1.5.4/CMakeLists.txt` & `pyhtml2md-1.6.0/CMakeLists.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 cmake_minimum_required(VERSION 3.8)
-project(html2md VERSION 1.5.4 LANGUAGES CXX)
+project(html2md VERSION 1.6.0 LANGUAGES CXX)
 
 set(PROJECT_HOMEPAGE_URL "https://tim-gromeyer.github.io/html2md/")
 set(html2md_HOMEPAGE_URL "${PROJECT_HOMEPAGE_URL}")
 
 set(PROJECT_DESCRIPTION "Transform your HTML into clean, easy-to-read markdown with html2md")
 set(html2md_DESCRIPTION "${PROJECT_DESCRIPTION}")
 
@@ -53,14 +53,17 @@
         cxx_auto_type # auto keyword
         cxx_constexpr # constexpr support
         cxx_range_for # for (auto test : tests)
         cxx_std_11 # Require at least c++11
     )
     target_compile_definitions(pyhtml2md PRIVATE PYTHON_BINDINGS)
     target_include_directories(pyhtml2md PRIVATE include)
+    if (SKBUILD)
+      install(TARGETS pyhtml2md DESTINATION "${SKBUILD_PLATLIB_DIR}")
+    endif()
     return()
 endif()
 
 add_library(html2md ${SOURCES})
 set_target_properties(html2md PROPERTIES
     VERSION ${PROJECT_VERSION}
     SOVERSION ${PROJECT_VERSION_MAJOR}
```

### Comparing `pyhtml2md-1.5.4/COPYING` & `pyhtml2md-1.6.0/COPYING`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/PKG-INFO` & `pyhtml2md-1.6.0/python/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: pyhtml2md
-Version: 1.5.4
-Summary: Transform your HTML into clean, easy-to-read markdown with pyhtml2md.
-Home-page: https://github.com/tim-gromeyer/html2md
-Author: Tim Gromeyer
-Author-email: sakul8826@gmail.com
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: COPYING
-Provides-Extra: test
-Requires-Dist: pytest>=6.0; extra == "test"
-
 # pyhtml2md
 
 pyhtml2md provides a way to use the html2md C++ library in Python. html2md is a fast and reliable library for converting HTML content into markdown.
 
 <div class="hidable-toc">
 
 - [Installation](#installation)
```

### Comparing `pyhtml2md-1.5.4/README.md` & `pyhtml2md-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/include/html2md.h` & `pyhtml2md-1.6.0/include/html2md.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 // Copyright (c) Tim Gromeyer
 // Licensed under the MIT License - https://opensource.org/licenses/MIT
 
 #ifndef HTML2MD_H
 #define HTML2MD_H
 
-#include <map>
 #include <memory>
 #include <string>
 #include <unordered_map>
-#include <vector>
 
 /*!
  * \brief html2md namespace
  *
  * The html2md namespace provides:
  * 1. The Converter class
  * 2. Static wrapper around Converter class
@@ -36,18 +34,32 @@
  * html2md::Converter c(html, options);
  * auto md = c.convert();
  * ```
  */
 struct Options {
   /*!
    * \brief Add new line when a certain number of characters is reached
+   *
+   * \see softBreak
+   * \see hardBreak
    */
   bool splitLines = true;
 
   /*!
+   * \brief softBreak Wrap after ...  characters when the next space is reached
+   * and as long as it's not in a list, table, image or anchor (link).
+   */
+  int softBreak = 80;
+
+  /*!
+   * \brief hardBreak Force a break after ... characters in a line
+   */
+  int hardBreak = 100;
+
+  /*!
    * \brief The char used for unordered lists
    *
    * Valid:
    * - `-`
    * - `+`
    * - `*`
    *
@@ -92,15 +104,16 @@
    * Whetever to format Markdown Tables.
    * Default is true.
    */
   bool formatTable = true;
 
   inline bool operator==(html2md::Options o) const {
     return splitLines == o.splitLines && unorderedList == o.unorderedList &&
-           orderedList == o.orderedList && includeTitle == o.includeTitle;
+           orderedList == o.orderedList && includeTitle == o.includeTitle &&
+           softBreak == o.softBreak && hardBreak == o.hardBreak;
   };
 };
 
 /*!
  * \brief Class for converting HTML to Markdown
  *
  * This class converts HTML to Markdown.
@@ -298,14 +311,15 @@
   bool is_in_code_ = false;
   bool is_in_list_ = false;
   bool is_in_p_ = false;
   bool is_in_pre_ = false;
   bool is_in_table_ = false;
   bool is_in_table_row_ = false;
   bool is_in_tag_ = false;
+  bool is_self_closing_tag_ = false;
 
   // relevant for <li> only, false = is in unordered list
   bool is_in_ordered_list_ = false;
   uint8_t index_ol = 0;
 
   // store the table start
   size_t table_start = 0;
```

### Comparing `pyhtml2md-1.5.4/pyhtml2md.egg-info/PKG-INFO` & `pyhtml2md-1.6.0/docs/index.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,123 +1,98 @@
-Metadata-Version: 2.1
-Name: pyhtml2md
-Version: 1.5.4
-Summary: Transform your HTML into clean, easy-to-read markdown with pyhtml2md.
-Home-page: https://github.com/tim-gromeyer/html2md
-Author: Tim Gromeyer
-Author-email: sakul8826@gmail.com
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: COPYING
-Provides-Extra: test
-Requires-Dist: pytest>=6.0; extra == "test"
-
-# pyhtml2md
-
-pyhtml2md provides a way to use the html2md C++ library in Python. html2md is a fast and reliable library for converting HTML content into markdown.
-
-<div class="hidable-toc">
-
-- [Installation](#installation)
-- [Basic usage](#basic-usage)
-- [Advanced usage](#advanced-usage)
-- [Supported Tags](#supported-tags)
-- [License](#license)
-
-</div>
-
-<div id="doxygen-toc" style="visibility:hidden">
+# html2md
 
 [TOC]
 
-</div>
+## What does it do
 
+html2md is a fast and reliable C++ library for converting HTML content into markdown. It offers support for a wide range of HTML tags, including those for formatting text, creating lists, and inserting images and links. In addition, html2md is the only HTML to markdown converter that offers support for table formatting, making it a valuable tool for users who need to convert HTML tables into markdown.
 
-## Installation
+## How to use this library
 
-You can install using pip:
+### CMake
 
-```bash
-pip3 install pyhtml2md
-```
+Install html2md. Either use the pre-built packages found on [GitHub releases](https://github.com/tim-gromeyer/html2md/releases) or build and install it yourself.
 
-## Basic usage
 
-Here is an example of how to use the pyhtml2md to convert HTML to markdown:
+Afterwards:
 
-```python
-import pyhtml2md
-
-markdown = pyhtml2md.convert("<h1>Hello, world!</h1>")
-print(markdown)
+```cmake
+find_package(html2md)
+target_link_library(your_target PRIVATE html2md)
 ```
 
-The `convert` function takes an HTML string as input and returns a markdown string.
+### Manually
 
-## Advanced usage
+To use html2md, follow these steps:
 
-pyhtml2md provides a `Options` class to customize the generation process.  
-You can find all information on the c++ [documentation](https://tim-gromeyer.github.io/html2md/index.html)
+1. Clone the library: `git clone https://github.com/tim-gromeyer/html2md`
+2. Add the files `include/html2md.h` and `src/html2md.cpp` to your project
+3. Include the `html2md.h` header in your code
+4. Use the `html2md::Convert` function to convert your HTML content into markdown
 
-Here is an example:
+Here is an example of how to use the `html2md::Convert` function:
 
-```python
-import pyhtml2md
+```cpp
+#include <html2md.h>
 
-options = pyhtml2md.Options()
-options.splitLines = False
+//...
 
-converter = pyhtml2md.Converter("<h1>Hello Python!</h1>", options)
-markdown = converter.convert()
-print(markdown)
-print(converter.ok())
+std::cout << html2md::Convert("<h1>foo</h1>"); // # foo
 ```
 
 ## Supported Tags
 
-pyhtml2md supports the following HTML tags:
+html2md supports the following HTML tags:
+
+
+| Tag          | Description        | Comment                                    |
+| ------------ | ------------------ | ------------------------------------------ |
+| `a`          | Anchor or link     | Supports the `href` and `name` attributes. |
+| `b`          | Bold               |                                            |
+| `blockquote` | Indented paragraph |                                            |
+| `br`         | Line break         |                                            |
+| `cite`       | Inline citation    | Same as `i`.                               |
+| `code`       | Code               |                                            |
+| `dd`         | Definition data    |                                            |
+| `del`        | Strikethrough      |                                            |
+| `dfn`        | Definition         | Same as `i`.                               |
+| `div`        | Document division  |                                            |
+| `em`         | Emphasized         | Same as `i`.                               |
+| `h1`         | Level 1 heading    |                                            |
+| `h2`         | Level 2 heading    |                                            |
+| `h3`         | Level 3 heading    |                                            |
+| `h4`         | Level 4 heading    |                                            |
+| `h5`         | Level 5 heading    |                                            |
+| `h6`         | Level 6 heading    |                                            |
+| `head`       | Document header    | Ignored.                                   |
+| `hr`         | Horizontal line    |                                            |
+| `i`          | Italic             |                                            |
+| `img`        | Image              | Supports the `src` and `alt` attributes.   |
+| `li`         | List item          |                                            |
+| `meta`       | Meta-information   | Ignored.                                   |
+| `ol`         | Ordered list       | Don't use other lists in this list.        |
+| `p`          | Paragraph          |                                            |
+| `pre`        | Preformatted text  | Works only with `code`.                    |
+| `s`          | Strikethrough      | Same as `del`.                             |
+| `span`       | Grouped elements   |                                            |
+| `strong`     | Strong             | Same as `b`.                               |
+| `table`      | Table              |                                            |
+| `td`         | Table data cell    | Uses `align` from `th`.                    |
+| `th`         | Table header cell  | Supports the `align` attribute.            |
+| `title`      | Document title     | Same as `h1`.                              |
+| `tr`         | Table row          |                                            |
+| `u`          | Underlined         | Uses HTML.                                 |
+| `ul`         | Unordered list     |                                            |
+
+## Bindings
+
+- [Python](../python/README.md)
+
+## Requirements
+
+1. A compiler with **c++11** support like *g++>=9*
 
-| Tag          | Description        | Comment                                             |
-|--------------|--------------------|-----------------------------------------------------|
-| `a`          | Anchor or link     | Supports the `href`, `name` and `title` attributes. |
-| `b`          | Bold               |                                                     |
-| `blockquote` | Indented paragraph |                                                     |
-| `br`         | Line break         |                                                     |
-| `cite`       | Inline citation    | Same as `i`.                                        |
-| `code`       | Code               |                                                     |
-| `dd`         | Definition data    |                                                     |
-| `del`        | Strikethrough      |                                                     |
-| `dfn`        | Definition         | Same as `i`.                                        |
-| `div`        | Document division  |                                                     |
-| `em`         | Emphasized         | Same as `i`.                                        |
-| `h1`         | Level 1 heading    |                                                     |
-| `h2`         | Level 2 heading    |                                                     |
-| `h3`         | Level 3 heading    |                                                     |
-| `h4`         | Level 4 heading    |                                                     |
-| `h5`         | Level 5 heading    |                                                     |
-| `h6`         | Level 6 heading    |                                                     |
-| `head`       | Document header    | Ignored.                                            |
-| `hr`         | Horizontal line    |                                                     |
-| `i`          | Italic             |                                                     |
-| `img`        | Image              | Supports `src`, `alt`, `title` attributes.          |
-| `li`         | List item          |                                                     |
-| `meta`       | Meta-information   | Ignored.                                            |
-| `ol`         | Ordered list       |                                                     |
-| `p`          | Paragraph          |                                                     |
-| `pre`        | Preformatted text  | Works only with `code`.                             |
-| `s`          | Strikethrough      | Same as `del`.                                      |
-| `span`       | Grouped elements   | Does nothing.                                       |
-| `strong`     | Strong             | Same as `b`.                                        |
-| `table`      | Table              | Tables are formatted!                               |
-| `tbody`      | Table body         | Does nothing.                                       |
-| `td`         | Table data cell    | Uses `align` from `th`.                             |
-| `tfoot`      | Table footer       | Does nothing.                                       |
-| `th`         | Table header cell  | Supports the `align` attribute.                     |
-| `thead`      | Table header       | Does nothing.                                       |
-| `title`      | Document title     | Same as `h1`.                                       |
-| `tr`         | Table row          |                                                     |
-| `u`          | Underlined         | Uses HTML.                                          |
-| `ul`         | Unordered list     |                                                     |
+That's all!
 
 ## License
 
-pyhtml2md is licensed under [The MIT License (MIT)](https://opensource.org/licenses/MIT)
+html2md is licensed under [The MIT License (MIT)](https://opensource.org/licenses/MIT)
```

### Comparing `pyhtml2md-1.5.4/python/README.md` & `pyhtml2md-1.6.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: pyhtml2md
+Version: 1.6.0
+Summary: Transform your HTML into clean, easy-to-read markdown with pyhtml2md.
+Keywords: html,markdown,html-to-markdown,python3,cpp17,cpp-library,html2markdown,html2md
+Author-Email: Tim Gromeyer <sakul8826@gmail.com>
+License: MIT
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: C++
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: File Formats
+Classifier: Topic :: Text Processing :: Markup :: Markdown
+Classifier: Topic :: Text Processing :: Markup :: HTML
+Project-URL: Repository, https://github.com/tim-gromeyer/html2md
+Requires-Python: >=3.7
+Provides-Extra: test
+Requires-Dist: pytest>=6.0; extra == "test"
+Description-Content-Type: text/markdown
+
 # pyhtml2md
 
 pyhtml2md provides a way to use the html2md C++ library in Python. html2md is a fast and reliable library for converting HTML content into markdown.
 
 <div class="hidable-toc">
 
 - [Installation](#installation)
```

### Comparing `pyhtml2md-1.5.4/python/bindings.cpp` & `pyhtml2md-1.6.0/python/bindings.cpp`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/CMakeLists.txt` & `pyhtml2md-1.6.0/python/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/LICENSE` & `pyhtml2md-1.6.0/python/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/include/pybind11/attr.h` & `pyhtml2md-1.6.0/python/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/include/pybind11/buffer_info.h` & `pyhtml2md-1.6.0/python/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/include/pybind11/cast.h` & `pyhtml2md-1.6.0/python/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/include/pybind11/chrono.h` & `pyhtml2md-1.6.0/python/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/include/pybind11/complex.h` & `pyhtml2md-1.6.0/python/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/include/pybind11/detail/class.h` & `pyhtml2md-1.6.0/python/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/include/pybind11/detail/common.h` & `pyhtml2md-1.6.0/python/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/include/pybind11/detail/descr.h` & `pyhtml2md-1.6.0/python/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/include/pybind11/detail/init.h` & `pyhtml2md-1.6.0/python/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/include/pybind11/detail/internals.h` & `pyhtml2md-1.6.0/python/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/include/pybind11/detail/type_caster_base.h` & `pyhtml2md-1.6.0/python/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/include/pybind11/detail/typeid.h` & `pyhtml2md-1.6.0/python/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/include/pybind11/eigen/matrix.h` & `pyhtml2md-1.6.0/python/pybind11/include/pybind11/eigen/matrix.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/include/pybind11/eigen/tensor.h` & `pyhtml2md-1.6.0/python/pybind11/include/pybind11/eigen/tensor.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/include/pybind11/embed.h` & `pyhtml2md-1.6.0/python/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/include/pybind11/eval.h` & `pyhtml2md-1.6.0/python/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/include/pybind11/functional.h` & `pyhtml2md-1.6.0/python/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/include/pybind11/gil.h` & `pyhtml2md-1.6.0/python/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/include/pybind11/gil_safe_call_once.h` & `pyhtml2md-1.6.0/python/pybind11/include/pybind11/gil_safe_call_once.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/include/pybind11/iostream.h` & `pyhtml2md-1.6.0/python/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/include/pybind11/numpy.h` & `pyhtml2md-1.6.0/python/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/include/pybind11/operators.h` & `pyhtml2md-1.6.0/python/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/include/pybind11/options.h` & `pyhtml2md-1.6.0/python/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/include/pybind11/pybind11.h` & `pyhtml2md-1.6.0/python/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/include/pybind11/pytypes.h` & `pyhtml2md-1.6.0/python/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/include/pybind11/stl/filesystem.h` & `pyhtml2md-1.6.0/python/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/include/pybind11/stl.h` & `pyhtml2md-1.6.0/python/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/include/pybind11/stl_bind.h` & `pyhtml2md-1.6.0/python/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/include/pybind11/type_caster_pyobject_ptr.h` & `pyhtml2md-1.6.0/python/pybind11/include/pybind11/type_caster_pyobject_ptr.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/include/pybind11/typing.h` & `pyhtml2md-1.6.0/python/pybind11/include/pybind11/typing.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/tools/FindCatch.cmake` & `pyhtml2md-1.6.0/python/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/tools/FindEigen3.cmake` & `pyhtml2md-1.6.0/python/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/tools/FindPythonLibsNew.cmake` & `pyhtml2md-1.6.0/python/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/tools/JoinPaths.cmake` & `pyhtml2md-1.6.0/python/pybind11/tools/JoinPaths.cmake`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/tools/check-style.sh` & `pyhtml2md-1.6.0/python/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/tools/cmake_uninstall.cmake.in` & `pyhtml2md-1.6.0/python/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/tools/codespell_ignore_lines_from_errors.py` & `pyhtml2md-1.6.0/python/pybind11/tools/codespell_ignore_lines_from_errors.py`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/tools/libsize.py` & `pyhtml2md-1.6.0/python/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/tools/make_changelog.py` & `pyhtml2md-1.6.0/python/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/tools/pybind11Common.cmake` & `pyhtml2md-1.6.0/python/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/tools/pybind11Config.cmake.in` & `pyhtml2md-1.6.0/python/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/tools/pybind11NewTools.cmake` & `pyhtml2md-1.6.0/python/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/tools/pybind11Tools.cmake` & `pyhtml2md-1.6.0/python/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/tools/setup_global.py.in` & `pyhtml2md-1.6.0/python/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/python/pybind11/tools/setup_main.py.in` & `pyhtml2md-1.6.0/python/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.5.4/src/html2md.cpp` & `pyhtml2md-1.6.0/src/html2md.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,17 @@
 // Licensed under the MIT License - https://opensource.org/licenses/MIT
 
 #include "html2md.h"
 #include "table.h"
 
 #include <algorithm>
 #include <cstring>
-#include <functional>
 #include <memory>
 #include <sstream>
-#include <stack>
-#include <utility>
+#include <vector>
 
 using std::make_shared;
 using std::string;
 using std::vector;
 
 namespace {
 bool startsWith(const string &str, const string &prefix) {
@@ -406,30 +404,28 @@
       prev_prev_ch_in_md_ = md_[md_.length() - 2];
   }
 
   return this;
 }
 
 bool Converter::ParseCharInTag(char ch) {
-  if (ch == '/' && current_tag_.empty()) {
-    is_closing_tag_ = true;
+  if (ch == '/' && !is_in_attribute_value_) {
+    is_closing_tag_ = current_tag_.empty();
+    is_self_closing_tag_ = !is_closing_tag_;
 
     return true;
   }
 
   if (ch == '>')
     return OnHasLeftTag();
 
-  if (ch == '=')
-    return true;
-
   if (ch == '"') {
     if (is_in_attribute_value_) {
       is_in_attribute_value_ = false;
-    } else if (prev_ch_in_md_ == '=') {
+    } else if (current_tag_[current_tag_.length() - 1] == '=') {
       is_in_attribute_value_ = true;
     }
 
     return true;
   }
 
   current_tag_ += ch;
@@ -449,20 +445,21 @@
   current_tag_ = Split(current_tag_, ' ')[0];
 
   auto tag = tags_[current_tag_];
 
   if (!tag)
     return true;
 
-  if (is_closing_tag_) {
+  if (!is_closing_tag_) {
+    tag->OnHasLeftOpeningTag(this);
+  }
+  if (is_closing_tag_ || is_self_closing_tag_) {
     is_closing_tag_ = false;
 
     tag->OnHasLeftClosingTag(this);
-  } else {
-    tag->OnHasLeftOpeningTag(this);
   }
 
   return true;
 }
 
 Converter *Converter::ShortenMarkdown(size_t chars) {
   md_ = md_.substr(0, md_.length() - chars);
@@ -513,21 +510,21 @@
     break;
   default:
     md_ += ch;
     ++chars_in_curr_line_;
     break;
   }
 
-  if (chars_in_curr_line_ > 80 && !is_in_table_ && !is_in_list_ &&
+  if (chars_in_curr_line_ > option.softBreak && !is_in_table_ && !is_in_list_ &&
       current_tag_ != kTagImg && current_tag_ != kTagAnchor &&
       option.splitLines) {
     if (ch == ' ') { // If the next char is - it will become a list
       md_ += '\n';
       chars_in_curr_line_ = 0;
-    } else if (chars_in_curr_line_ > 100) {
+    } else if (chars_in_curr_line_ > option.hardBreak) {
       ReplacePreviousSpaceInLineByNewline();
     }
   }
 
   return false;
 }
```

### Comparing `pyhtml2md-1.5.4/src/table.cpp` & `pyhtml2md-1.6.0/src/table.cpp`

 * *Files identical despite different names*

