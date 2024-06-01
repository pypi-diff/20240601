# Comparing `tmp/cmdix-3.1.1.tar.gz` & `tmp/cmdix-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmdix-3.1.1.tar", last modified: Wed Dec 20 17:18:20 2023, max compression
+gzip compressed data, was "cmdix-3.1.2.tar", last modified: Sat Jun  1 00:42:12 2024, max compression
```

## Comparing `cmdix-3.1.1.tar` & `cmdix-3.1.2.tar`

### file list

```diff
@@ -1,123 +1,124 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 17:18:20.028279 cmdix-3.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2023-12-20 17:18:01.000000 cmdix-3.1.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      246 2023-12-20 17:18:01.000000 cmdix-3.1.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 17:18:20.008279 cmdix-3.1.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2023-12-20 17:18:01.000000 cmdix-3.1.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 17:18:20.008279 cmdix-3.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2774 2023-12-20 17:18:01.000000 cmdix-3.1.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)       81 2023-12-20 17:18:01.000000 cmdix-3.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      188 2023-12-20 17:18:01.000000 cmdix-3.1.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      556 2023-12-20 17:18:01.000000 cmdix-3.1.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2023-12-20 17:18:01.000000 cmdix-3.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2023-12-20 17:18:01.000000 cmdix-3.1.1/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2783 2023-12-20 17:18:20.028279 cmdix-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2023-12-20 17:18:01.000000 cmdix-3.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 17:18:20.008279 cmdix-3.1.1/cmdix/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4752 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       53 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 17:18:20.020279 cmdix-3.1.1/cmdix/command/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/arch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/base64.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/basename.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/bunzip2.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/bzip2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/cal.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/cat.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/chmod.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/chown.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/chroot.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/clear.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/cp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3479 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/crond.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/diff.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/dirname.py
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/expand.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/gunzip.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/gzip.py
--rw-r--r--   0 runner    (1001) docker     (127)    11171 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/httpd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/id.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/init.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/kill.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/ln.py
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/ls.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/md5sum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/mkdir.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/mktemp.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/more.py
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/mount.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/mv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/nl.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/pwd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/rm.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/rmdir.py
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/sendmail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/seq.py
--rw-r--r--   0 runner    (1001) docker     (127)     4103 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/sh.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/sha1sum.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/sha224sum.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/sha256sum.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/sha384sum.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/sha512sum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/shred.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/shuf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/sleep.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/sort.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/tail.py
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/tar.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/tee.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/touch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4196 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/uname.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/uptime.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/uuidgen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/watch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/wc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/wget.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/whoami.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/yes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/command/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 17:18:20.020279 cmdix-3.1.1/cmdix/compat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/compat/py39.py
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/compressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/hasher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5340 2023-12-20 17:18:01.000000 cmdix-3.1.1/cmdix/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 17:18:20.024279 cmdix-3.1.1/cmdix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2783 2023-12-20 17:18:19.000000 cmdix-3.1.1/cmdix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2023-12-20 17:18:20.000000 cmdix-3.1.1/cmdix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-20 17:18:19.000000 cmdix-3.1.1/cmdix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2023-12-20 17:18:19.000000 cmdix-3.1.1/cmdix.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      370 2023-12-20 17:18:19.000000 cmdix-3.1.1/cmdix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-20 17:18:19.000000 cmdix-3.1.1/cmdix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      192 2023-12-20 17:18:01.000000 cmdix-3.1.1/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 17:18:20.020279 cmdix-3.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2023-12-20 17:18:01.000000 cmdix-3.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-12-20 17:18:01.000000 cmdix-3.1.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      329 2023-12-20 17:18:01.000000 cmdix-3.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-12-20 17:18:01.000000 cmdix-3.1.1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-20 17:18:01.000000 cmdix-3.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      946 2023-12-20 17:18:01.000000 cmdix-3.1.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2023-12-20 17:18:20.028279 cmdix-3.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 17:18:20.024279 cmdix-3.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2023-12-20 17:18:01.000000 cmdix-3.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2023-12-20 17:18:01.000000 cmdix-3.1.1/tests/test_base64.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2023-12-20 17:18:01.000000 cmdix-3.1.1/tests/test_basename.py
--rw-r--r--   0 runner    (1001) docker     (127)     7017 2023-12-20 17:18:01.000000 cmdix-3.1.1/tests/test_cal.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2023-12-20 17:18:01.000000 cmdix-3.1.1/tests/test_cat.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2023-12-20 17:18:01.000000 cmdix-3.1.1/tests/test_cp.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2023-12-20 17:18:01.000000 cmdix-3.1.1/tests/test_env.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2023-12-20 17:18:01.000000 cmdix-3.1.1/tests/test_expand.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2023-12-20 17:18:01.000000 cmdix-3.1.1/tests/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2023-12-20 17:18:01.000000 cmdix-3.1.1/tests/test_md5sum.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2023-12-20 17:18:01.000000 cmdix-3.1.1/tests/test_nl.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2023-12-20 17:18:01.000000 cmdix-3.1.1/tests/test_onlyunix.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2023-12-20 17:18:01.000000 cmdix-3.1.1/tests/test_pycoreutils.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2023-12-20 17:18:01.000000 cmdix-3.1.1/tests/test_pycoreutils_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2023-12-20 17:18:01.000000 cmdix-3.1.1/tests/test_tail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2023-12-20 17:18:01.000000 cmdix-3.1.1/tests/test_tar.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2023-12-20 17:18:01.000000 cmdix-3.1.1/tests/test_uuidgen.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-20 17:18:01.000000 cmdix-3.1.1/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2023-12-20 17:18:01.000000 cmdix-3.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:42:12.519266 cmdix-3.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-06-01 00:41:54.000000 cmdix-3.1.2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-06-01 00:41:54.000000 cmdix-3.1.2/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:42:12.499266 cmdix-3.1.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-06-01 00:41:54.000000 cmdix-3.1.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:42:12.499266 cmdix-3.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-06-01 00:41:54.000000 cmdix-3.1.2/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-06-01 00:41:54.000000 cmdix-3.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-06-01 00:41:54.000000 cmdix-3.1.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-06-01 00:41:54.000000 cmdix-3.1.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-06-01 00:41:54.000000 cmdix-3.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-06-01 00:41:54.000000 cmdix-3.1.2/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-06-01 00:42:12.519266 cmdix-3.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-06-01 00:41:54.000000 cmdix-3.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:42:12.499266 cmdix-3.1.2/cmdix/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4752 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       53 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:42:12.511266 cmdix-3.1.2/cmdix/command/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/arch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/base64.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/basename.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/bunzip2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/bzip2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/cal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/cat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/chmod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/chown.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/chroot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/clear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/cp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/crond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/dirname.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/expand.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/gunzip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/gzip.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11149 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/httpd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/kill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/ln.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/md5sum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/mkdir.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/mktemp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/mount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/mv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/nl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/pwd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/rmdir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/sendmail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/seq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/sh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/sha1sum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/sha224sum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/sha256sum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/sha384sum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/sha512sum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/shred.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/shuf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/sleep.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/tail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/tar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/tee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/touch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/uname.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/uptime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/uuidgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/watch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/wc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/wget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/whoami.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/yes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/command/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:42:12.511266 cmdix-3.1.2/cmdix/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/compat/py39.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/compressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/hasher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-06-01 00:41:54.000000 cmdix-3.1.2/cmdix/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:42:12.515266 cmdix-3.1.2/cmdix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-06-01 00:42:12.000000 cmdix-3.1.2/cmdix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-06-01 00:42:12.000000 cmdix-3.1.2/cmdix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 00:42:12.000000 cmdix-3.1.2/cmdix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-06-01 00:42:12.000000 cmdix-3.1.2/cmdix.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-06-01 00:42:12.000000 cmdix-3.1.2/cmdix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-01 00:42:12.000000 cmdix-3.1.2/cmdix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-06-01 00:41:54.000000 cmdix-3.1.2/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:42:12.511266 cmdix-3.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-06-01 00:41:54.000000 cmdix-3.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-06-01 00:41:54.000000 cmdix-3.1.2/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-06-01 00:41:54.000000 cmdix-3.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-06-01 00:41:54.000000 cmdix-3.1.2/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-06-01 00:41:54.000000 cmdix-3.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-06-01 00:41:54.000000 cmdix-3.1.2/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-06-01 00:41:54.000000 cmdix-3.1.2/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 00:42:12.519266 cmdix-3.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:42:12.515266 cmdix-3.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-06-01 00:41:54.000000 cmdix-3.1.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-06-01 00:41:54.000000 cmdix-3.1.2/tests/test_base64.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-06-01 00:41:54.000000 cmdix-3.1.2/tests/test_basename.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7017 2024-06-01 00:41:54.000000 cmdix-3.1.2/tests/test_cal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-06-01 00:41:54.000000 cmdix-3.1.2/tests/test_cat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-06-01 00:41:54.000000 cmdix-3.1.2/tests/test_cp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-06-01 00:41:54.000000 cmdix-3.1.2/tests/test_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-06-01 00:41:54.000000 cmdix-3.1.2/tests/test_expand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-06-01 00:41:54.000000 cmdix-3.1.2/tests/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-06-01 00:41:54.000000 cmdix-3.1.2/tests/test_md5sum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-06-01 00:41:54.000000 cmdix-3.1.2/tests/test_nl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-06-01 00:41:54.000000 cmdix-3.1.2/tests/test_onlyunix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-06-01 00:41:54.000000 cmdix-3.1.2/tests/test_pycoreutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-06-01 00:41:54.000000 cmdix-3.1.2/tests/test_pycoreutils_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-06-01 00:41:54.000000 cmdix-3.1.2/tests/test_tail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-06-01 00:41:54.000000 cmdix-3.1.2/tests/test_tar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-06-01 00:41:54.000000 cmdix-3.1.2/tests/test_uuidgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-06-01 00:41:54.000000 cmdix-3.1.2/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-06-01 00:41:54.000000 cmdix-3.1.2/tox.ini
```

### Comparing `cmdix-3.1.1/.github/workflows/main.yml` & `cmdix-3.1.2/.github/workflows/main.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 name: tests
 
-on: [push, pull_request]
+on:
+  merge_group:
+  push:
+    branches-ignore:
+    # temporary GH branches relating to merge queues (jaraco/skeleton#93)
+    - gh-readonly-queue/**
+    tags:
+    # required if branches-ignore is supplied (jaraco/skeleton#103)
+    - '**'
+  pull_request:
 
 permissions:
   contents: read
 
 env:
   # Environment variable to support color support (jaraco/skeleton#66)
   FORCE_COLOR: 1
@@ -18,28 +27,30 @@
   TOX_OVERRIDE: >-
     testenv.pass_env+=GITHUB_*,FORCE_COLOR
 
 
 jobs:
   test:
     strategy:
+      # https://blog.jaraco.com/efficient-use-of-ci-resources/
       matrix:
         python:
         - "3.8"
-        - "3.11"
         - "3.12"
         platform:
         - ubuntu-latest
         - macos-latest
         - windows-latest
         include:
         - python: "3.9"
           platform: ubuntu-latest
         - python: "3.10"
           platform: ubuntu-latest
+        - python: "3.11"
+          platform: ubuntu-latest
         # disabled for #11
         #- python: pypy3.10
         #  platform: ubuntu-latest
         
         # tests hang on Python < 3.9
         exclude:
         - python: "3.8"
@@ -60,15 +71,17 @@
       - name: Run
         run: tox
 
   collateral:
     strategy:
       fail-fast: false
       matrix:
-        job: [diffcov, docs]
+        job:
+        - diffcov
+        - docs
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0
       - name: Setup Python
         uses: actions/setup-python@v4
```

### Comparing `cmdix-3.1.1/Dockerfile` & `cmdix-3.1.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/LICENSE` & `cmdix-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/NEWS.rst` & `cmdix-3.1.2/NEWS.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v3.1.2
+======
+
+Bugfixes
+--------
+
+- Add support for listing files by name. (#16)
+
+
 v3.1.1
 ======
 
 Bugfixes
 --------
 
 - env now honors ``-`` and options in the command (#14)
```

### Comparing `cmdix-3.1.1/PKG-INFO` & `cmdix-3.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,65 +1,59 @@
 Metadata-Version: 2.1
 Name: cmdix
-Version: 3.1.1
+Version: 3.1.2
 Summary: Unix commands in Pure Python
-Home-page: https://github.com/jaraco/cmdix
-Author: Jason R. Coombs
-Author-email: jaraco@jaraco.com
+Author-email: "Jason R. Coombs" <jaraco@jaraco.com>
+Project-URL: Homepage, https://github.com/jaraco/cmdix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Environment :: Console
 Classifier: Topic :: System :: Shells
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: importlib_resources
 Requires-Dist: backports.hook_compressed; python_version < "3.10"
 Requires-Dist: more_itertools
-Provides-Extra: testing
-Requires-Dist: pytest>=6; extra == "testing"
-Requires-Dist: pytest-checkdocs>=2.4; extra == "testing"
-Requires-Dist: pytest-black>=0.3.7; platform_python_implementation != "PyPy" and extra == "testing"
-Requires-Dist: pytest-cov; extra == "testing"
-Requires-Dist: pytest-mypy>=0.9.1; platform_python_implementation != "PyPy" and extra == "testing"
-Requires-Dist: pytest-enabler>=2.2; extra == "testing"
-Requires-Dist: pytest-ruff; extra == "testing"
-Requires-Dist: types-backports; extra == "testing"
-Provides-Extra: docs
-Requires-Dist: sphinx>=3.5; extra == "docs"
-Requires-Dist: sphinx<7.2.5; extra == "docs"
-Requires-Dist: jaraco.packaging>=9.3; extra == "docs"
-Requires-Dist: rst.linker>=1.9; extra == "docs"
-Requires-Dist: furo; extra == "docs"
-Requires-Dist: sphinx-lint; extra == "docs"
+Provides-Extra: test
+Requires-Dist: pytest!=8.1.*,>=6; extra == "test"
+Requires-Dist: pytest-checkdocs>=2.4; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: pytest-mypy; extra == "test"
+Requires-Dist: pytest-enabler>=2.2; extra == "test"
+Requires-Dist: pytest-ruff>=0.2.1; extra == "test"
+Requires-Dist: types-backports; extra == "test"
+Provides-Extra: doc
+Requires-Dist: sphinx>=3.5; extra == "doc"
+Requires-Dist: jaraco.packaging>=9.3; extra == "doc"
+Requires-Dist: rst.linker>=1.9; extra == "doc"
+Requires-Dist: furo; extra == "doc"
+Requires-Dist: sphinx-lint; extra == "doc"
 
 .. image:: https://img.shields.io/pypi/v/cmdix.svg
    :target: https://pypi.org/project/cmdix
 
 .. image:: https://img.shields.io/pypi/pyversions/cmdix.svg
 
 .. image:: https://github.com/jaraco/cmdix/actions/workflows/main.yml/badge.svg
    :target: https://github.com/jaraco/cmdix/actions?query=workflow%3A%22tests%22
    :alt: tests
 
 .. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
     :target: https://github.com/astral-sh/ruff
     :alt: Ruff
 
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/psf/black
-   :alt: Code style: Black
-
 .. image:: https://readthedocs.org/projects/cmdix/badge/?version=latest
    :target: https://cmdix.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2023-informational
+.. image:: https://img.shields.io/badge/skeleton-2024-informational
    :target: https://blog.jaraco.com/skeleton
 
 cmdix is a pure Python implementation of various standard UNIX commands,
 like 'ls', 'cp' and 'sleep'. It also contains a shell-like environment which
 will make Unix-users feel right at home on the Windows command-prompt.
 
 Forked from the abandoned `pycoreutils project
```

### Comparing `cmdix-3.1.1/README.rst` & `cmdix-3.1.2/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -7,22 +7,18 @@
    :target: https://github.com/jaraco/cmdix/actions?query=workflow%3A%22tests%22
    :alt: tests
 
 .. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
     :target: https://github.com/astral-sh/ruff
     :alt: Ruff
 
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/psf/black
-   :alt: Code style: Black
-
 .. image:: https://readthedocs.org/projects/cmdix/badge/?version=latest
    :target: https://cmdix.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2023-informational
+.. image:: https://img.shields.io/badge/skeleton-2024-informational
    :target: https://blog.jaraco.com/skeleton
 
 cmdix is a pure Python implementation of various standard UNIX commands,
 like 'ls', 'cp' and 'sleep'. It also contains a shell-like environment which
 will make Unix-users feel right at home on the Windows command-prompt.
 
 Forked from the abandoned `pycoreutils project
```

### Comparing `cmdix-3.1.1/cmdix/__init__.py` & `cmdix-3.1.2/cmdix/__init__.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/command/base64.py` & `cmdix-3.1.2/cmdix/command/base64.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/command/basename.py` & `cmdix-3.1.2/cmdix/command/basename.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/command/cal.py` & `cmdix-3.1.2/cmdix/command/cal.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/command/cat.py` & `cmdix-3.1.2/cmdix/command/cat.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/command/chmod.py` & `cmdix-3.1.2/cmdix/command/chmod.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/command/chown.py` & `cmdix-3.1.2/cmdix/command/chown.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/command/chroot.py` & `cmdix-3.1.2/cmdix/command/chroot.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/command/cp.py` & `cmdix-3.1.2/cmdix/command/cp.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/command/crond.py` & `cmdix-3.1.2/cmdix/command/crond.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/command/diff.py` & `cmdix-3.1.2/cmdix/command/diff.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/command/dirname.py` & `cmdix-3.1.2/cmdix/command/dirname.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/command/env.py` & `cmdix-3.1.2/cmdix/command/env.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,16 +46,15 @@
             return self.__saved
         except AttributeError:
             if result := self._check(input):
                 self.__saved = result
             return result
 
     @abc.abstractmethod
-    def _check(self, input):
-        ...  # pragma: no cover
+    def _check(self, input): ...  # pragma: no cover
 
 
 class VarsCheck(Latching):
     """
     Partition inputs to env into vars and cmd args.
 
     >>> vars, cmd = VarsCheck().partition(['foo=bar', 'bing=baz', 'blue', 'z=3'])
```

### Comparing `cmdix-3.1.1/cmdix/command/expand.py` & `cmdix-3.1.2/cmdix/command/expand.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/command/httpd.py` & `cmdix-3.1.2/cmdix/command/httpd.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,17 +79,15 @@
 def wsgierror(start_response, code, text, headers=[]):
     h = [(b'Content-Type', b'text/html')]
     h.extend(headers)
     start_response(b'{} '.format(code), h)
     return [
         b'''<!DOCTYPE HTML PUBLIC "-//IETF//DTD HTML 2.0//EN"><html><head>
                 <title>{code} {text}</title></head><body><h1>{code} {text}</h1>
-                </body></html>'''.format(
-            code=code, text=text
-        )
+                </body></html>'''.format(code=code, text=text)
     ]
 
 
 def wsgiserver(app, args):
     """
     Parse opts and return a WSGIServer running app
     """
```

### Comparing `cmdix-3.1.1/cmdix/command/id.py` & `cmdix-3.1.2/cmdix/command/id.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/command/init.py` & `cmdix-3.1.2/cmdix/command/init.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/command/kill.py` & `cmdix-3.1.2/cmdix/command/kill.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/command/ln.py` & `cmdix-3.1.2/cmdix/command/ln.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/command/logger.py` & `cmdix-3.1.2/cmdix/command/logger.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/command/mkdir.py` & `cmdix-3.1.2/cmdix/command/mkdir.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/command/mktemp.py` & `cmdix-3.1.2/cmdix/command/mktemp.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/command/more.py` & `cmdix-3.1.2/cmdix/command/more.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/command/mount.py` & `cmdix-3.1.2/cmdix/command/mount.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/command/mv.py` & `cmdix-3.1.2/cmdix/command/mv.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/command/nl.py` & `cmdix-3.1.2/cmdix/command/nl.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/command/pwd.py` & `cmdix-3.1.2/cmdix/command/pwd.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/command/rm.py` & `cmdix-3.1.2/cmdix/command/rm.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/command/rmdir.py` & `cmdix-3.1.2/cmdix/command/rmdir.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/command/sendmail.py` & `cmdix-3.1.2/cmdix/command/sendmail.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/command/seq.py` & `cmdix-3.1.2/cmdix/command/seq.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/command/sh.py` & `cmdix-3.1.2/cmdix/command/sh.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,17 +41,15 @@
     prompttemplate = '{username}@{hostname}:{currentpath}$ '
 
     def __init__(self, nocoreutils=False, *args, **kwargs):
         if not nocoreutils:
             # Copy all commands from cmdix to 'do_foo' functions
             for command in cmdix.listcommands():
                 x = """self.do_{0} = lambda l: \
-                       cmdix.runcommandline('{0} '+ l)""".format(
-                    command
-                )
+                       cmdix.runcommandline('{0} '+ l)""".format(command)
                 exec(x)
         return cmd.Cmd.__init__(self, *args, **kwargs)
 
     def default(self, line):
         """
         Called on an input line when the command prefix is not recognized.
         """
```

### Comparing `cmdix-3.1.1/cmdix/command/shred.py` & `cmdix-3.1.2/cmdix/command/shred.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/command/shuf.py` & `cmdix-3.1.2/cmdix/command/shuf.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/command/sleep.py` & `cmdix-3.1.2/cmdix/command/sleep.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/command/sort.py` & `cmdix-3.1.2/cmdix/command/sort.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/command/tail.py` & `cmdix-3.1.2/cmdix/command/tail.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/command/tar.py` & `cmdix-3.1.2/cmdix/command/tar.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/command/tee.py` & `cmdix-3.1.2/cmdix/command/tee.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/command/touch.py` & `cmdix-3.1.2/cmdix/command/touch.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/command/uname.py` & `cmdix-3.1.2/cmdix/command/uname.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/command/uptime.py` & `cmdix-3.1.2/cmdix/command/uptime.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/command/uuidgen.py` & `cmdix-3.1.2/cmdix/command/uuidgen.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/command/watch.py` & `cmdix-3.1.2/cmdix/command/watch.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/command/wc.py` & `cmdix-3.1.2/cmdix/command/wc.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/command/wget.py` & `cmdix-3.1.2/cmdix/command/wget.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/command/zip.py` & `cmdix-3.1.2/cmdix/command/zip.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/compressor.py` & `cmdix-3.1.2/cmdix/compressor.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/exception.py` & `cmdix-3.1.2/cmdix/exception.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/hasher.py` & `cmdix-3.1.2/cmdix/hasher.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix/lib.py` & `cmdix-3.1.2/cmdix/lib.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/cmdix.egg-info/PKG-INFO` & `cmdix-3.1.2/cmdix.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,65 +1,59 @@
 Metadata-Version: 2.1
 Name: cmdix
-Version: 3.1.1
+Version: 3.1.2
 Summary: Unix commands in Pure Python
-Home-page: https://github.com/jaraco/cmdix
-Author: Jason R. Coombs
-Author-email: jaraco@jaraco.com
+Author-email: "Jason R. Coombs" <jaraco@jaraco.com>
+Project-URL: Homepage, https://github.com/jaraco/cmdix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Environment :: Console
 Classifier: Topic :: System :: Shells
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: importlib_resources
 Requires-Dist: backports.hook_compressed; python_version < "3.10"
 Requires-Dist: more_itertools
-Provides-Extra: testing
-Requires-Dist: pytest>=6; extra == "testing"
-Requires-Dist: pytest-checkdocs>=2.4; extra == "testing"
-Requires-Dist: pytest-black>=0.3.7; platform_python_implementation != "PyPy" and extra == "testing"
-Requires-Dist: pytest-cov; extra == "testing"
-Requires-Dist: pytest-mypy>=0.9.1; platform_python_implementation != "PyPy" and extra == "testing"
-Requires-Dist: pytest-enabler>=2.2; extra == "testing"
-Requires-Dist: pytest-ruff; extra == "testing"
-Requires-Dist: types-backports; extra == "testing"
-Provides-Extra: docs
-Requires-Dist: sphinx>=3.5; extra == "docs"
-Requires-Dist: sphinx<7.2.5; extra == "docs"
-Requires-Dist: jaraco.packaging>=9.3; extra == "docs"
-Requires-Dist: rst.linker>=1.9; extra == "docs"
-Requires-Dist: furo; extra == "docs"
-Requires-Dist: sphinx-lint; extra == "docs"
+Provides-Extra: test
+Requires-Dist: pytest!=8.1.*,>=6; extra == "test"
+Requires-Dist: pytest-checkdocs>=2.4; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: pytest-mypy; extra == "test"
+Requires-Dist: pytest-enabler>=2.2; extra == "test"
+Requires-Dist: pytest-ruff>=0.2.1; extra == "test"
+Requires-Dist: types-backports; extra == "test"
+Provides-Extra: doc
+Requires-Dist: sphinx>=3.5; extra == "doc"
+Requires-Dist: jaraco.packaging>=9.3; extra == "doc"
+Requires-Dist: rst.linker>=1.9; extra == "doc"
+Requires-Dist: furo; extra == "doc"
+Requires-Dist: sphinx-lint; extra == "doc"
 
 .. image:: https://img.shields.io/pypi/v/cmdix.svg
    :target: https://pypi.org/project/cmdix
 
 .. image:: https://img.shields.io/pypi/pyversions/cmdix.svg
 
 .. image:: https://github.com/jaraco/cmdix/actions/workflows/main.yml/badge.svg
    :target: https://github.com/jaraco/cmdix/actions?query=workflow%3A%22tests%22
    :alt: tests
 
 .. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
     :target: https://github.com/astral-sh/ruff
     :alt: Ruff
 
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/psf/black
-   :alt: Code style: Black
-
 .. image:: https://readthedocs.org/projects/cmdix/badge/?version=latest
    :target: https://cmdix.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2023-informational
+.. image:: https://img.shields.io/badge/skeleton-2024-informational
    :target: https://blog.jaraco.com/skeleton
 
 cmdix is a pure Python implementation of various standard UNIX commands,
 like 'ls', 'cp' and 'sleep'. It also contains a shell-like environment which
 will make Unix-users feel right at home on the Windows command-prompt.
 
 Forked from the abandoned `pycoreutils project
```

### Comparing `cmdix-3.1.1/cmdix.egg-info/SOURCES.txt` & `cmdix-3.1.2/cmdix.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 LICENSE
 NEWS.rst
 README.rst
 conftest.py
 mypy.ini
 pyproject.toml
 pytest.ini
-setup.cfg
+ruff.toml
 towncrier.toml
 tox.ini
 .github/dependabot.yml
 .github/workflows/main.yml
 cmdix/__init__.py
 cmdix/__main__.py
 cmdix/compressor.py
```

### Comparing `cmdix-3.1.1/cmdix.egg-info/entry_points.txt` & `cmdix-3.1.2/cmdix.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/docs/conf.py` & `cmdix-3.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/tests/__init__.py` & `cmdix-3.1.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/tests/test_base64.py` & `cmdix-3.1.2/tests/test_base64.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/tests/test_cal.py` & `cmdix-3.1.2/tests/test_cal.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/tests/test_cat.py` & `cmdix-3.1.2/tests/test_cat.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/tests/test_cp.py` & `cmdix-3.1.2/tests/test_cp.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/tests/test_env.py` & `cmdix-3.1.2/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/tests/test_ls.py` & `cmdix-3.1.2/tests/test_ls.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,26 +9,31 @@
 
 class TestCase(BaseTestCase):
     def test_ls(self, capsys):
         self.setup_filesystem()
         self.runcommandline('ls')
         assert capsys.readouterr().out == 'dir1\ndir2\nfile1\nfile2.txt\nfile3.empty\n'
 
+    def test_ls_file(self, capsys):
+        self.setup_filesystem()
+        self.runcommandline('ls file2.txt')
+        assert capsys.readouterr().out == 'file2.txt\n'
+
     @pytest.mark.xfail("platform.system() == 'Windows'")
     def test_ls_l(self, capsys):
         os.mkdir('biz', mode=0o755)
         self.createfile('foo', size=100)
         self.createfile('bar', size=999999)
         os.chmod('bar', stat.S_IWUSR + stat.S_IRGRP + stat.S_IWOTH + stat.S_IXOTH)
         os.chmod('foo', 0o644)
 
         dirsize = os.stat('biz').st_size
         uid = os.getuid()
         gid = os.getgid()
-        date = time.strftime('%Y-%m-%d %H:%m', time.localtime())
+        date = time.strftime('%Y-%m-%d %H:%M', time.localtime())
         self.runcommandline('ls -l')
         expected = (
             textwrap.dedent(
                 """
             --w-r---wx 1 {uid:<5} {gid:<5} 999999 {date} bar
             drwxr-xr-x 2 {uid:<5} {gid:<5} {dirsize:>6} {date} biz
             -rw-r--r-- 1 {uid:<5} {gid:<5}    100 {date} foo
```

### Comparing `cmdix-3.1.1/tests/test_nl.py` & `cmdix-3.1.2/tests/test_nl.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/tests/test_onlyunix.py` & `cmdix-3.1.2/tests/test_onlyunix.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/tests/test_tar.py` & `cmdix-3.1.2/tests/test_tar.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/tests/test_uuidgen.py` & `cmdix-3.1.2/tests/test_uuidgen.py`

 * *Files identical despite different names*

### Comparing `cmdix-3.1.1/tox.ini` & `cmdix-3.1.2/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -3,30 +3,31 @@
 deps =
 setenv =
 	PYTHONWARNDEFAULTENCODING = 1
 commands =
 	pytest {posargs}
 usedevelop = True
 extras =
-	testing
+	test
 
 [testenv:diffcov]
 description = run tests and check that diff from main is covered
 deps =
+	{[testenv]deps}
 	diff-cover
 commands =
 	pytest {posargs} --cov-report xml
 	diff-cover coverage.xml --compare-branch=origin/main --html-report diffcov.html
 	diff-cover coverage.xml --compare-branch=origin/main --fail-under=100
 
 [testenv:docs]
 description = build the documentation
 extras =
-	docs
-	testing
+	doc
+	test
 changedir = docs
 commands =
 	python -m sphinx -W --keep-going . {toxinidir}/build/html
 	python -m sphinxlint \
 		# workaround for sphinx-contrib/sphinx-lint#83
 		--jobs 1
```

