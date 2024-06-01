# Comparing `tmp/sphinx-conestack-theme-1.0b2.tar.gz` & `tmp/sphinx-conestack-theme-1.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sphinx-conestack-theme-1.0b2.tar", last modified: Tue Sep 21 11:31:37 2021, max compression
+gzip compressed data, was "dist/sphinx-conestack-theme-1.0b3.tar", last modified: Mon Dec 13 08:04:36 2021, max compression
```

## Comparing `sphinx-conestack-theme-1.0b2.tar` & `sphinx-conestack-theme-1.0b3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2021-09-21 11:31:37.000000 sphinx-conestack-theme-1.0b2/
--rw-r--r--   0 rnix      (1000) rnix      (1000)      256 2021-09-21 11:28:46.000000 sphinx-conestack-theme-1.0b2/CHANGES.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1317 2021-08-17 07:24:08.000000 sphinx-conestack-theme-1.0b2/LICENSE.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)      166 2021-09-21 11:23:12.000000 sphinx-conestack-theme-1.0b2/MANIFEST.in
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3878 2021-09-21 11:31:37.000000 sphinx-conestack-theme-1.0b2/PKG-INFO
--rw-r--r--   0 rnix      (1000) rnix      (1000)      889 2021-09-21 11:27:17.000000 sphinx-conestack-theme-1.0b2/README.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)       38 2021-09-21 11:31:37.000000 sphinx-conestack-theme-1.0b2/setup.cfg
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1316 2021-09-21 11:31:17.000000 sphinx-conestack-theme-1.0b2/setup.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2021-09-21 11:31:37.000000 sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2720 2021-08-27 06:22:11.000000 sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/__init__.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2021-09-21 11:31:37.000000 sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/
--rw-r--r--   0 rnix      (1000) rnix      (1000)      390 2021-08-27 11:59:09.000000 sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/external.html
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1169 2021-08-27 06:22:11.000000 sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/footer.html
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1200 2021-08-27 06:22:11.000000 sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/github.html
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4729 2021-08-27 06:22:11.000000 sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/gitlab.html
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2280 2021-08-27 06:22:11.000000 sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/layout.html
--rw-r--r--   0 rnix      (1000) rnix      (1000)      279 2021-08-23 10:09:28.000000 sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/localtoc.html
--rw-r--r--   0 rnix      (1000) rnix      (1000)      306 2021-08-27 06:22:11.000000 sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/logo.html
--rw-r--r--   0 rnix      (1000) rnix      (1000)       99 2021-08-23 05:01:18.000000 sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/mobiletoc.html
--rw-r--r--   0 rnix      (1000) rnix      (1000)       97 2021-08-23 05:01:18.000000 sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/navigationtoc.html
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1799 2021-09-21 11:23:12.000000 sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/npm.html
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2683 2021-08-27 06:22:11.000000 sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/pypi.html
--rw-r--r--   0 rnix      (1000) rnix      (1000)      526 2021-08-27 06:22:11.000000 sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/relations.html
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1407 2021-08-23 05:10:52.000000 sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/search.html
--rw-r--r--   0 rnix      (1000) rnix      (1000)      601 2021-08-23 13:20:39.000000 sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/searchbox.html
--rw-r--r--   0 rnix      (1000) rnix      (1000)      253 2021-08-23 05:01:18.000000 sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/sidebar.html
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2021-09-21 11:31:37.000000 sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/static/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2021-09-21 11:31:37.000000 sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/static/bootstrap-icons/
--rw-r--r--   0 rnix      (1000) rnix      (1000)    65696 2021-08-20 11:09:46.000000 sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/static/bootstrap-icons/bootstrap-icons.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)    34982 2021-08-20 11:09:46.000000 sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/static/bootstrap-icons/bootstrap-icons.json
--rw-r--r--   0 rnix      (1000) rnix      (1000)   726419 2021-08-20 11:09:46.000000 sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/static/bootstrap-icons/bootstrap-icons.svg
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2021-09-21 11:31:37.000000 sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/static/bootstrap-icons/fonts/
--rw-r--r--   0 rnix      (1000) rnix      (1000)   120468 2021-08-20 11:09:46.000000 sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/static/bootstrap-icons/fonts/bootstrap-icons.woff
--rw-r--r--   0 rnix      (1000) rnix      (1000)    90528 2021-08-20 11:09:46.000000 sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/static/bootstrap-icons/fonts/bootstrap-icons.woff2
--rw-r--r--   0 rnix      (1000) rnix      (1000)    78468 2021-08-23 05:01:18.000000 sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/static/bootstrap.bundle.min.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)   327261 2021-08-19 12:01:33.000000 sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/static/bootstrap.bundle.min.js.map
--rw-r--r--   0 rnix      (1000) rnix      (1000)   204136 2021-08-17 07:37:33.000000 sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/static/bootstrap.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)   536547 2021-08-17 07:37:33.000000 sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/static/bootstrap.css.map
--rw-r--r--   0 rnix      (1000) rnix      (1000)      150 2021-08-27 06:52:04.000000 sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/static/conestack-vars.css_t
--rw-r--r--   0 rnix      (1000) rnix      (1000)    18708 2021-09-21 11:30:04.000000 sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/static/conestack.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3919 2021-09-21 11:30:04.000000 sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/static/conestack.css.map
--rw-r--r--   0 rnix      (1000) rnix      (1000)     5548 2021-09-21 11:29:24.000000 sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/static/conestack.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3482 2021-08-23 05:01:18.000000 sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/static/conestack.svg
--rw-r--r--   0 rnix      (1000) rnix      (1000)      352 2021-09-21 11:23:12.000000 sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/theme.conf
--rw-r--r--   0 rnix      (1000) rnix      (1000)      949 2021-08-27 06:22:11.000000 sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/twitter.html
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2021-09-21 11:31:37.000000 sphinx-conestack-theme-1.0b2/sphinx_conestack_theme.egg-info/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3878 2021-09-21 11:31:37.000000 sphinx-conestack-theme-1.0b2/sphinx_conestack_theme.egg-info/PKG-INFO
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2112 2021-09-21 11:31:37.000000 sphinx-conestack-theme-1.0b2/sphinx_conestack_theme.egg-info/SOURCES.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2021-09-21 11:31:37.000000 sphinx-conestack-theme-1.0b2/sphinx_conestack_theme.egg-info/dependency_links.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)       57 2021-09-21 11:31:37.000000 sphinx-conestack-theme-1.0b2/sphinx_conestack_theme.egg-info/entry_points.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2021-08-17 08:35:26.000000 sphinx-conestack-theme-1.0b2/sphinx_conestack_theme.egg-info/not-zip-safe
--rw-r--r--   0 rnix      (1000) rnix      (1000)        7 2021-09-21 11:31:37.000000 sphinx-conestack-theme-1.0b2/sphinx_conestack_theme.egg-info/requires.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)       23 2021-09-21 11:31:37.000000 sphinx-conestack-theme-1.0b2/sphinx_conestack_theme.egg-info/top_level.txt
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2021-12-13 08:04:36.000000 sphinx-conestack-theme-1.0b3/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      400 2021-12-13 07:59:04.000000 sphinx-conestack-theme-1.0b3/CHANGES.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1317 2021-08-17 07:24:08.000000 sphinx-conestack-theme-1.0b3/LICENSE.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      166 2021-09-21 11:23:12.000000 sphinx-conestack-theme-1.0b3/MANIFEST.in
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4102 2021-12-13 08:04:36.000000 sphinx-conestack-theme-1.0b3/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      889 2021-09-21 11:27:17.000000 sphinx-conestack-theme-1.0b3/README.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       38 2021-12-13 08:04:36.000000 sphinx-conestack-theme-1.0b3/setup.cfg
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1316 2021-12-13 08:01:24.000000 sphinx-conestack-theme-1.0b3/setup.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2021-12-13 08:04:36.000000 sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2720 2021-08-27 06:22:11.000000 sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/__init__.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2021-12-13 08:04:36.000000 sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      390 2021-08-27 11:59:09.000000 sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/external.html
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1169 2021-08-27 06:22:11.000000 sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/footer.html
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1200 2021-08-27 06:22:11.000000 sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/github.html
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4729 2021-08-27 06:22:11.000000 sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/gitlab.html
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2463 2021-09-27 08:16:12.000000 sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/layout.html
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      279 2021-08-23 10:09:28.000000 sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/localtoc.html
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      306 2021-08-27 06:22:11.000000 sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/logo.html
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       99 2021-08-23 05:01:18.000000 sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/mobiletoc.html
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       97 2021-08-23 05:01:18.000000 sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/navigationtoc.html
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1799 2021-09-21 11:23:12.000000 sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/npm.html
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2683 2021-08-27 06:22:11.000000 sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/pypi.html
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      526 2021-08-27 06:22:11.000000 sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/relations.html
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1407 2021-08-23 05:10:52.000000 sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/search.html
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      601 2021-08-23 13:20:39.000000 sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/searchbox.html
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      253 2021-08-23 05:01:18.000000 sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/sidebar.html
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2021-12-13 08:04:36.000000 sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/static/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2021-12-13 08:04:36.000000 sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/static/bootstrap-icons/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    65696 2021-08-20 11:09:46.000000 sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/static/bootstrap-icons/bootstrap-icons.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    34982 2021-08-20 11:09:46.000000 sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/static/bootstrap-icons/bootstrap-icons.json
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   726419 2021-08-20 11:09:46.000000 sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/static/bootstrap-icons/bootstrap-icons.svg
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2021-12-13 08:04:36.000000 sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/static/bootstrap-icons/fonts/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   120468 2021-08-20 11:09:46.000000 sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/static/bootstrap-icons/fonts/bootstrap-icons.woff
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    90528 2021-08-20 11:09:46.000000 sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/static/bootstrap-icons/fonts/bootstrap-icons.woff2
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    78468 2021-08-23 05:01:18.000000 sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/static/bootstrap.bundle.min.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   327261 2021-08-19 12:01:33.000000 sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/static/bootstrap.bundle.min.js.map
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   204136 2021-08-17 07:37:33.000000 sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/static/bootstrap.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   536547 2021-08-17 07:37:33.000000 sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/static/bootstrap.css.map
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      315 2021-09-27 08:16:12.000000 sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/static/conestack-vars.css_t
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    19039 2021-12-13 08:00:04.000000 sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/static/conestack.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3984 2021-12-13 08:00:04.000000 sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/static/conestack.css.map
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5548 2021-09-21 11:29:24.000000 sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/static/conestack.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3482 2021-08-23 05:01:18.000000 sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/static/conestack.svg
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      451 2021-09-27 08:16:12.000000 sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/theme.conf
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      949 2021-08-27 06:22:11.000000 sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/twitter.html
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2021-12-13 08:04:36.000000 sphinx-conestack-theme-1.0b3/sphinx_conestack_theme.egg-info/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4102 2021-12-13 08:04:35.000000 sphinx-conestack-theme-1.0b3/sphinx_conestack_theme.egg-info/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2112 2021-12-13 08:04:35.000000 sphinx-conestack-theme-1.0b3/sphinx_conestack_theme.egg-info/SOURCES.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2021-12-13 08:04:35.000000 sphinx-conestack-theme-1.0b3/sphinx_conestack_theme.egg-info/dependency_links.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       57 2021-12-13 08:04:35.000000 sphinx-conestack-theme-1.0b3/sphinx_conestack_theme.egg-info/entry_points.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2021-08-17 08:35:26.000000 sphinx-conestack-theme-1.0b3/sphinx_conestack_theme.egg-info/not-zip-safe
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        7 2021-12-13 08:04:35.000000 sphinx-conestack-theme-1.0b3/sphinx_conestack_theme.egg-info/requires.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       23 2021-12-13 08:04:35.000000 sphinx-conestack-theme-1.0b3/sphinx_conestack_theme.egg-info/top_level.txt
```

### Comparing `sphinx-conestack-theme-1.0b2/LICENSE.rst` & `sphinx-conestack-theme-1.0b3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `sphinx-conestack-theme-1.0b2/PKG-INFO` & `sphinx-conestack-theme-1.0b3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: sphinx-conestack-theme
-Version: 1.0b2
+Version: 1.0b3
 Summary: Mobile friendly Bootstrap 5 based Sphinx theme
 Home-page: https://github.com/conestack/sphinx-conestack-theme
 Author: Cone Contributors
 Author-email: dev@conestack.org
 License: Simplified BSD
 Description: Conestack Sphinx Theme
         ======================
@@ -47,14 +47,24 @@
         
         - Robert Niederreiter
         
         
         Changes
         =======
         
+        1.0b3 (unreleased)
+        ------------------
+        
+        - Add theme option to hide localtoc.
+        
+        - Improve global toc styles.
+        
+        - Make colums widths configurable.
+        
+        
         1.0b2 (2021-09-21)
         ------------------
         
         - Add "scroll to top" button on mobile devices.
         
         - Remove "copy to clipboard" button on mobile devices.
```

### Comparing `sphinx-conestack-theme-1.0b2/README.rst` & `sphinx-conestack-theme-1.0b3/README.rst`

 * *Files identical despite different names*

### Comparing `sphinx-conestack-theme-1.0b2/setup.py` & `sphinx-conestack-theme-1.0b3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 def read_file(name):
     with open(os.path.join(os.path.dirname(__file__), name)) as f:
         return f.read()
 
 
-version = '1.0b2'
+version = '1.0b3'
 shortdesc = 'Mobile friendly Bootstrap 5 based Sphinx theme'
 longdesc = '\n\n'.join([read_file(name) for name in [
     'README.rst',
     'CHANGES.rst',
     'LICENSE.rst'
 ]])
```

### Comparing `sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/__init__.py` & `sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/footer.html` & `sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/footer.html`

 * *Files identical despite different names*

### Comparing `sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/github.html` & `sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/github.html`

 * *Files identical despite different names*

### Comparing `sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/gitlab.html` & `sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/gitlab.html`

 * *Files identical despite different names*

### Comparing `sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/layout.html` & `sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/layout.html`

 * *Files 8% similar despite different names*

```diff
@@ -56,22 +56,28 @@
   {% endblock %}
 
   <div class="container-xxl my-md-4" id="cs-layout">
     {% block sidebar %}
       {%- include "sidebar.html" %}
     {% endblock %}
 
-    <main class="document cs-main order-1">
+    {% if theme_sidebar_right %}
+      <main class="document cs-main order-1">
+    {% else %}
+      <main class="document cs-main d-block overflow-auto order-1">
+    {% endif %}
       {%- block document %}
       <div class="ps-lg-4 mt-3 cs-content">
         {% block body %}{% endblock %}
       </div>
       {%- endblock %}
 
+    {% if theme_sidebar_right %}
       {%- include "localtoc.html" %}
+    {% endif %}
     </main>
   </div>
 {%- endblock %}
 
 {% block footer %}
   {%- include "footer.html" %}
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,12 +1,13 @@
 {%- extends "basic/layout.html" %} {%- block extrahead %}
 {% endblock %} {% block relbar1 %}{% endblock %} {% block content %}
 {% block header_navbar %} {%- include "logo.html" %} {% block searchbox %} {%-
 include "searchbox.html" %} {% endblock %} {%- include "external.html" %}
 {%- include "mobiletoc.html" %}
 {% endblock %}
-{% block sidebar %} {%- include "sidebar.html" %} {% endblock %} {%- block
-document %}
+{% block sidebar %} {%- include "sidebar.html" %} {% endblock %} {% if
+theme_sidebar_right %} {% else %} {% endif %} {%- block document %}
 {% block body %}{% endblock %}
-{%- endblock %} {%- include "localtoc.html" %}
+{%- endblock %} {% if theme_sidebar_right %} {%- include "localtoc.html" %} {%
+endif %}
 {%- endblock %} {% block footer %} {%- include "footer.html" %} {% endblock %}
 {%- block relbar2 %}{% endblock %}
```

### Comparing `sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/npm.html` & `sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/npm.html`

 * *Files identical despite different names*

### Comparing `sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/pypi.html` & `sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/pypi.html`

 * *Files identical despite different names*

### Comparing `sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/relations.html` & `sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/relations.html`

 * *Files identical despite different names*

### Comparing `sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/search.html` & `sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/search.html`

 * *Files identical despite different names*

### Comparing `sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/searchbox.html` & `sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/searchbox.html`

 * *Files identical despite different names*

### Comparing `sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/static/bootstrap-icons/bootstrap-icons.css` & `sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/static/bootstrap-icons/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/static/bootstrap-icons/bootstrap-icons.json` & `sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/static/bootstrap-icons/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/static/bootstrap-icons/bootstrap-icons.svg` & `sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/static/bootstrap-icons/bootstrap-icons.svg`

 * *Files identical despite different names*

### Comparing `sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/static/bootstrap-icons/fonts/bootstrap-icons.woff` & `sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/static/bootstrap-icons/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/static/bootstrap-icons/fonts/bootstrap-icons.woff2` & `sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/static/bootstrap-icons/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/static/bootstrap.bundle.min.js` & `sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/static/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/static/bootstrap.bundle.min.js.map` & `sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/static/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/static/bootstrap.css` & `sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/static/bootstrap.css`

 * *Files identical despite different names*

### Comparing `sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/static/bootstrap.css.map` & `sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/static/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/static/conestack.css` & `sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/static/conestack.css`

 * *Files 2% similar despite different names*

```diff
@@ -172,14 +172,16 @@
 .cs-nav-toc ul ul {
   padding-left: 1.2rem;
 }
 .cs-nav-toc li.toctree-l1 {
   position: relative;
   font-weight: 600;
   margin-bottom: 0.3rem;
+  margin-left: 20px;
+  text-indent: -10px;
 }
 .cs-nav-toc li.toctree-l1.current > a {
   color: var(--cs-bg-color);
 }
 .cs-nav-toc li.toctree-l1.current ul {
   display: block;
 }
@@ -209,14 +211,19 @@
 }
 .cs-nav-toc li.toctree-l1 > a.collapsed::before {
   content: "\f285" !important;
 }
 .cs-nav-toc li.toctree-l1 > span.toggle {
   position: absolute;
   cursor: pointer;
+  display: block;
+  width: 20px;
+  height: 20px;
+  left: -22px;
+  top: 2px;
 }
 .cs-nav-toc li.toctree-l1 > span.toggle::before {
   display: inline-block;
   font-family: bootstrap-icons !important;
   font-style: normal;
   font-weight: normal !important;
   font-variant: normal;
@@ -240,15 +247,15 @@
 }
 
 #cs-layout {
   min-height: calc(100vh - 19rem);
 }
 @media (min-width: 992px) {
   #cs-layout {
-    grid-template-columns: 1fr 5fr !important;
+    grid-template-columns: 1fr 10fr !important;
   }
 }
 @media (min-width: 769px) {
   #cs-layout {
     display: grid;
     gap: 1.5rem;
     grid-template-areas: "sidebar main";
@@ -257,14 +264,23 @@
 }
 @media (max-width: 768px) {
   #cs-layout {
     padding: 1rem;
   }
 }
 
+@media (min-width: 992px) {
+  #cs-layout, #cs-nav {
+    max-width: var(--layout-width) !important;
+  }
+
+  #cs-sidebar {
+    min-width: var(--sidebar-left-width) !important;
+  }
+}
 .cs-main {
   gap: inherit;
   display: grid;
   grid-area: main;
   grid-template-areas: "content toc";
   grid-template-columns: minmax(0, 4fr) 1fr;
   height: min-content;
@@ -610,15 +626,15 @@
     right: 0;
     z-index: 2;
     overflow-y: auto;
     min-height: calc(100vh - 30rem);
     height: max-content;
     max-height: calc(100vh - 8rem);
     width: min-content;
-    min-width: 180px;
+    min-width: var(--sidebar-right-width) !important;
   }
 }
 .cs-local-toc nav {
   font-size: 0.875rem;
 }
 .cs-local-toc nav ul {
   padding-left: 0;
```

### Comparing `sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/static/conestack.css.map` & `sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/static/conestack.css.map`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'mappings'": "';AAgBQ;AACA;AACA;AClBR;EACE;;;ACDF;EACE;EACA;EACA;EACA;;AAEA;EACE;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;;;AAKF;EAIE;EACA;EACA;EACA;EACA;;AAGF;EAZF;IAaI;;;AAGF;EAhBF;IAiBI;;;AAGF;EACE;;AAGF;EACE;;;AAIJ;EACE;;AAEA;EAHF;IAII;IACA;IACA;;;AAGF;EACE;;;AAKF;EADF;IAEI;;;AAEF;EAJF;IAKI;;;AAGF;EACE;;AAGF;EACE;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;;AAGF;EACE;;AAGF;EACE;;;AAIJ;EACE;EACA;;;AAGF;EACE;EACA;;AAEA;EAJF;IAKI;;;AAGF;EACE;;AAGF;EACE;;AAEA;EACE;EACA;EACA;;AAEA;EACE;EACA;EACA;;AAEA;EACE […]*

```diff
@@ -1,10 +1,10 @@
 {
     "file": "conestack.css",
-    "mappings": ";AAgBQ;AACA;AACA;AClBR;EACE;;;ACDF;EACE;EACA;EACA;EACA;;AAEA;EACE;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;;;AAKF;EAIE;EACA;EACA;EACA;EACA;;AAGF;EAZF;IAaI;;;AAGF;EAhBF;IAiBI;;;AAGF;EACE;;AAGF;EACE;;;AAIJ;EACE;;AAEA;EAHF;IAII;IACA;IACA;;;AAGF;EACE;;;AAKF;EADF;IAEI;;;AAEF;EAJF;IAKI;;;AAGF;EACE;;AAGF;EACE;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;;AAGF;EACE;;AAGF;EACE;;;AAIJ;EACE;EACA;;;AAGF;EACE;EACA;;AAEA;EAJF;IAKI;;;AAGF;EACE;;AAGF;EACE;;AAEA;EACE;EACA;EACA;;AAEA;EACE;EACA;EACA;;AAEA;EACE;EACA;;AAGF;EACE;;;AClIV;EACE;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;;AAEA;EAXF;IAYM;;;;AAKJ;EADF;IAEI;IACA;IACA;IACA;;;AAGF;AAAA;AAAA;AAAA;EAIE;EACA;;AAGF;EACE;EACA;EACA;;AAGF;EACE;;AAGF;EACE;EACA;EACA;;AAGE;EACE;;AAGF;EACE;;AAIJ;EACE;;AAGF;EACE;;AAKA;ECpEJ;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;ED8DM;EACA;EACA;;AAGF;EAEE;;AAGF;EACE;;AAIJ;EACE;EACA;;AAEA;EC1FJ;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EDoFM;EACA;;AAMJ;EACE;;AAEA;EAIE;;AAKF;EAIE;EACA;;;AEtHR;EACE;;AAEA;EAHF;IAII;;;AAGF;EAPF;IAQI;IACA;IACA;IACA;;;AAGF;EAdF;IAeI;;;;ACfJ;EACE;EACA;EACA;EACA;EACA;EACA;;AAEA;EARF;IASI;IACA;;;AAGF;EACE;;;AAIJ;EACE;EACA;;AAEA;EACE;EACA;;AAGF;EACE;EACA;EACA;EACA;;AAGF;EACE;;AAGF;AAAA;EAEE;EACA;EACA;EACA;;AAGF;EACE;EACA;EACA;EACA;;AAGF;EACE;;AAGF;EACE;EACA;EACA;EACA;;AAGE;EACE;;;AAMR;EACE;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;;;AClFA;EACE;;AAGF;EACE;;;AAIJ;EACE;IACE;;;ACXF;EACE;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;;AAEA;EACE;EACA;EACA;EACA;EACA;EACA;EACA;;AAEA;EACE;EACA;EACA;EACA;EACA;EACA;;AAMJ;EASE;;AARA;EACE;;AAEA;EACE;EACA;;AAMN;EASE;;AARA;EACE;;AAEA;EACE;EACA;;AAMN;EASE;;AARA;EACE;;AAEA;EACE;EACA;;AAMN;EASE;;AARA;EACE;;AAEA;EACE;EACA;;AAMN;EASE;;AARA;EACE;;AAEA;EACE;EACA;;AAMN;EASE;;AARA;EACE;;AAEA;EACE;EACA;;AAMN;EASE;;AARA;EACE;;AAEA;EACE;EACA;;AAMN;EASE;;AARA;EACE;;AAEA;EACE;EACA;;AAMN;EASE;;AARA;EACE;;AAEA;EACE;EACA;;;ACtIR;EACE;EACA;EACA;EACA;EACA;EACA;;AAEA;EACE;;AAGF;EACE;;AAGF;EACE;EACA;;AAGF;EACE;EACA;EACA;;AAEA;EACE;;AACA;EACE;;AAGJ;EACE;;AAIJ;EACE;;AAGF;EACE;EACA;EACA;EACA;;AAEA;EACE;;AAGF;EACE;EACA;EACA;;AAEA;EACE;EACA;;AAIJ;AAAA;EAEE;;AAEF;EACE;;;ACnEN;AAAA;EAEE;;AAKA;EACE;EACA;EACA;;AAGF;EACE;EACA;EACA;EACA;EACA;;AAEA;EACE;;AAGF;EACE;EACA;;AAEA;EACE;EACA;EACA;EACA;;AAGF;EACE;;AAGF;EACE;;;ACxCR;AAAA;AAAA;AAAA;AAAA;AAAA;AAAA;AAAA;EAQE;EACA;EACA;;AAGF;EACE;EACA;;AAGF;EACE;EACA;;AAGF;EACE;EACA;;AAGF;EACE;EACA;;;AC9BJ;EACE;EACA;;AAEA;EAJF;IAKI;;;AAGF;EARF;IASI;IACA;IACA;IACA;IACA;IACA;IACA;IACA;IACA;IACA;;;AAGF;EACE;;AAEA;EACE;EACE;;AAEA;EACE;EACA;;AAIJ;EACE;;AAGF;EACE;;AACA;EACE;;AAEF;EACE;;;AC5CR;EACE;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;;AAEA;EACE;EACA;EACA;;AAGF;EACE;EACA;;AAGF;EACE;;AAGF;EACE;;;AC3BJ;EACE;EACA;;AAGF;EACE;EACA;EACA;EACA;;AAEA;AAAA;AAAA;AAAA;AAAA;AAAA;EAME;EACA;;AAIA;EACE;;AACA;EACE;;AAKF;EACE;;AAGF;EACE;;AAKN;EACE;EACA;EACA;;;AC3CJ;EACE;EACA;;AAGF;AAAA;EAEE;EACA;EACA;EACA;;AAGF;EACE;;AAGF;EACE;EACA;;AAGF;EACE;;AAGF;EACE;EACA;EACA;EACA;;AAEA;EACE;;AAIJ;EACE;EACA;;AAGF;EACE;;AAGF;EACE;EACA;;AAGF;EACE;;AAGF;EACE;EACA;;AAGF;EACE;EACA;EACA;EACA;EACA;;AAGF;EACE;EACA;EACA;EACA;EACA;;AAGF;EACE;;AAIA;EACE;EACA;EACA;EACA;EACA;;AAGF;EACE;EACA;EACA;EACA;EACA;;AAGF;EACE;EACA;;AAIJ;EACE;EACA;EACA;EACA;EACA;EACA;EACA;EACA;;AAGF;EACE;EACA;EACA;EACA;EACA;;;ACvHF;EACE;EACA;EACA;;AAGF;AAAA;EAEE;EACA;EACA;EACA;EACA;EACA;;AAEA;AAAA;EACE;EACA;EACA;EACA;EACA;EACA;;AAEA;AAAA;EACE;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;;AAKN;EACE;EACA;EACA;EACA;EACA;EACA",
+    "mappings": ";AAgBQ;AACA;AACA;AClBR;EACE;;;ACDF;EACE;EACA;EACA;EACA;;AAEA;EACE;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;;;AAKF;EAIE;EACA;EACA;EACA;EACA;;AAGF;EAZF;IAaI;;;AAGF;EAhBF;IAiBI;;;AAGF;EACE;;AAGF;EACE;;;AAIJ;EACE;;AAEA;EAHF;IAII;IACA;IACA;;;AAGF;EACE;;;AAKF;EADF;IAEI;;;AAEF;EAJF;IAKI;;;AAGF;EACE;;AAGF;EACE;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;;AAGF;EACE;;AAGF;EACE;;;AAIJ;EACE;EACA;;;AAGF;EACE;EACA;;AAEA;EAJF;IAKI;;;AAGF;EACE;;AAGF;EACE;;AAEA;EACE;EACA;EACA;;AAEA;EACE;EACA;EACA;;AAEA;EACE;EACA;;AAGF;EACE;;;AClIV;EACE;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;;AAEA;EAXF;IAYM;;;;AAKJ;EADF;IAEI;IACA;IACA;IACA;;;AAGF;AAAA;AAAA;AAAA;EAIE;EACA;;AAGF;EACE;EACA;EACA;;AAGF;EACE;;AAGF;EACE;EACA;EACA;EACA;EACA;;AAGE;EACE;;AAGF;EACE;;AAIJ;EACE;;AAGF;EACE;;AAKA;ECtEJ;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EDgEM;EACA;EACA;;AAGF;EAEE;;AAGF;EACE;;AAIJ;EACE;EACA;EACA;EACA;EACA;EACA;EACA;;AAEA;ECjGJ;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;ED2FM;EACA;;AAMJ;EACE;;AAEA;EAIE;;AAKF;EAIE;EACA;;;AE7HR;EACE;;AAEA;EAHF;IAII;;;AAGF;EAPF;IAQI;IACA;IACA;IACA;;;AAGF;EAdF;IAeI;;;;AAIJ;EACE;IACE;;;EAGF;IACE;;;ACzBJ;EACE;EACA;EACA;EACA;EACA;EACA;;AAEA;EARF;IASI;IACA;;;AAGF;EACE;;;AAIJ;EACE;EACA;;AAEA;EACE;EACA;;AAGF;EACE;EACA;EACA;EACA;;AAGF;EACE;;AAGF;AAAA;EAEE;EACA;EACA;EACA;;AAGF;EACE;EACA;EACA;EACA;;AAGF;EACE;;AAGF;EACE;EACA;EACA;EACA;;AAGE;EACE;;;AAMR;EACE;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;;;AClFA;EACE;;AAGF;EACE;;;AAIJ;EACE;IACE;;;ACXF;EACE;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;;AAEA;EACE;EACA;EACA;EACA;EACA;EACA;EACA;;AAEA;EACE;EACA;EACA;EACA;EACA;EACA;;AAMJ;EASE;;AARA;EACE;;AAEA;EACE;EACA;;AAMN;EASE;;AARA;EACE;;AAEA;EACE;EACA;;AAMN;EASE;;AARA;EACE;;AAEA;EACE;EACA;;AAMN;EASE;;AARA;EACE;;AAEA;EACE;EACA;;AAMN;EASE;;AARA;EACE;;AAEA;EACE;EACA;;AAMN;EASE;;AARA;EACE;;AAEA;EACE;EACA;;AAMN;EASE;;AARA;EACE;;AAEA;EACE;EACA;;AAMN;EASE;;AARA;EACE;;AAEA;EACE;EACA;;AAMN;EASE;;AARA;EACE;;AAEA;EACE;EACA;;;ACtIR;EACE;EACA;EACA;EACA;EACA;EACA;;AAEA;EACE;;AAGF;EACE;;AAGF;EACE;EACA;;AAGF;EACE;EACA;EACA;;AAEA;EACE;;AACA;EACE;;AAGJ;EACE;;AAIJ;EACE;;AAGF;EACE;EACA;EACA;EACA;;AAEA;EACE;;AAGF;EACE;EACA;EACA;;AAEA;EACE;EACA;;AAIJ;AAAA;EAEE;;AAEF;EACE;;;ACnEN;AAAA;EAEE;;AAKA;EACE;EACA;EACA;;AAGF;EACE;EACA;EACA;EACA;EACA;;AAEA;EACE;;AAGF;EACE;EACA;;AAEA;EACE;EACA;EACA;EACA;;AAGF;EACE;;AAGF;EACE;;;ACxCR;AAAA;AAAA;AAAA;AAAA;AAAA;AAAA;AAAA;EAQE;EACA;EACA;;AAGF;EACE;EACA;;AAGF;EACE;EACA;;AAGF;EACE;EACA;;AAGF;EACE;EACA;;;AC9BJ;EACE;EACA;;AAEA;EAJF;IAKI;;;AAGF;EARF;IASI;IACA;IACA;IACA;IACA;IACA;IACA;IACA;IACA;IACA;;;AAGF;EACE;;AAEA;EACE;EACE;;AAEA;EACE;EACA;;AAIJ;EACE;;AAGF;EACE;;AACA;EACE;;AAEF;EACE;;;AC5CR;EACE;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;;AAEA;EACE;EACA;EACA;;AAGF;EACE;EACA;;AAGF;EACE;;AAGF;EACE;;;AC3BJ;EACE;EACA;;AAGF;EACE;EACA;EACA;EACA;;AAEA;AAAA;AAAA;AAAA;AAAA;AAAA;EAME;EACA;;AAIA;EACE;;AACA;EACE;;AAKF;EACE;;AAGF;EACE;;AAKN;EACE;EACA;EACA;;;AC3CJ;EACE;EACA;;AAGF;AAAA;EAEE;EACA;EACA;EACA;;AAGF;EACE;;AAGF;EACE;EACA;;AAGF;EACE;;AAGF;EACE;EACA;EACA;EACA;;AAEA;EACE;;AAIJ;EACE;EACA;;AAGF;EACE;;AAGF;EACE;EACA;;AAGF;EACE;;AAGF;EACE;EACA;;AAGF;EACE;EACA;EACA;EACA;EACA;;AAGF;EACE;EACA;EACA;EACA;EACA;;AAGF;EACE;;AAIA;EACE;EACA;EACA;EACA;EACA;;AAGF;EACE;EACA;EACA;EACA;EACA;;AAGF;EACE;EACA;;AAIJ;EACE;EACA;EACA;EACA;EACA;EACA;EACA;EACA;;AAGF;EACE;EACA;EACA;EACA;EACA;;;ACvHF;EACE;EACA;EACA;;AAGF;AAAA;EAEE;EACA;EACA;EACA;EACA;EACA;;AAEA;AAAA;EACE;EACA;EACA;EACA;EACA;EACA;;AAEA;AAAA;EACE;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;;AAKN;EACE;EACA;EACA;EACA;EACA;EACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "../scss/conestack.scss",
         "../scss/base.scss",
         "../scss/header.scss",
         "../scss/sidebar.scss",
```

### Comparing `sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/static/conestack.js` & `sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/static/conestack.js`

 * *Files identical despite different names*

### Comparing `sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/static/conestack.svg` & `sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/static/conestack.svg`

 * *Files identical despite different names*

### Comparing `sphinx-conestack-theme-1.0b2/sphinx_conestack_theme/conestack/twitter.html` & `sphinx-conestack-theme-1.0b3/sphinx_conestack_theme/conestack/twitter.html`

 * *Files identical despite different names*

### Comparing `sphinx-conestack-theme-1.0b2/sphinx_conestack_theme.egg-info/PKG-INFO` & `sphinx-conestack-theme-1.0b3/sphinx_conestack_theme.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: sphinx-conestack-theme
-Version: 1.0b2
+Version: 1.0b3
 Summary: Mobile friendly Bootstrap 5 based Sphinx theme
 Home-page: https://github.com/conestack/sphinx-conestack-theme
 Author: Cone Contributors
 Author-email: dev@conestack.org
 License: Simplified BSD
 Description: Conestack Sphinx Theme
         ======================
@@ -47,14 +47,24 @@
         
         - Robert Niederreiter
         
         
         Changes
         =======
         
+        1.0b3 (unreleased)
+        ------------------
+        
+        - Add theme option to hide localtoc.
+        
+        - Improve global toc styles.
+        
+        - Make colums widths configurable.
+        
+        
         1.0b2 (2021-09-21)
         ------------------
         
         - Add "scroll to top" button on mobile devices.
         
         - Remove "copy to clipboard" button on mobile devices.
```

### Comparing `sphinx-conestack-theme-1.0b2/sphinx_conestack_theme.egg-info/SOURCES.txt` & `sphinx-conestack-theme-1.0b3/sphinx_conestack_theme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

