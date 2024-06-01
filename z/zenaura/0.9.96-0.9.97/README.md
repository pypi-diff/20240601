# Comparing `tmp/zenaura-0.9.96.tar.gz` & `tmp/zenaura-0.9.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zenaura-0.9.96.tar", last modified: Thu May 30 13:46:28 2024, max compression
+gzip compressed data, was "zenaura-0.9.97.tar", last modified: Sat Jun  1 17:55:36 2024, max compression
```

## Comparing `zenaura-0.9.96.tar` & `zenaura-0.9.97.tar`

### file list

```diff
@@ -1,79 +1,77 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 13:46:28.591237 zenaura-0.9.96/
--rw-rw-rw-   0        0        0     1100 2024-05-11 11:29:30.000000 zenaura-0.9.96/LICENSE
--rw-rw-rw-   0        0        0     2028 2024-05-30 13:46:28.590736 zenaura-0.9.96/PKG-INFO
--rw-rw-rw-   0        0        0     1376 2024-05-26 16:54:28.000000 zenaura-0.9.96/README.md
--rw-rw-rw-   0        0        0       42 2024-05-30 13:46:28.591237 zenaura-0.9.96/setup.cfg
--rw-rw-rw-   0        0        0     1135 2024-05-30 13:45:51.000000 zenaura-0.9.96/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:46:28.555248 zenaura-0.9.96/tests/
--rw-rw-rw-   0        0        0    33440 2024-05-26 17:44:57.000000 zenaura-0.9.96/tests/test_algorithm.py
--rw-rw-rw-   0        0        0     6595 2024-05-27 20:30:05.000000 zenaura-0.9.96/tests/test_app.py
--rw-rw-rw-   0        0        0     7595 2024-05-26 17:44:57.000000 zenaura-0.9.96/tests/test_compiler.py
--rw-rw-rw-   0        0        0     4161 2024-05-26 17:44:57.000000 zenaura-0.9.96/tests/test_component_e2e.py
--rw-rw-rw-   0        0        0     1415 2024-05-26 17:44:57.000000 zenaura-0.9.96/tests/test_component_unit.py
--rw-rw-rw-   0        0        0     5301 2024-05-26 17:44:57.000000 zenaura-0.9.96/tests/test_node_properties.py
--rw-rw-rw-   0        0        0     1435 2024-05-26 17:44:57.000000 zenaura-0.9.96/tests/test_observer.py
--rw-rw-rw-   0        0        0     5710 2024-05-26 17:44:57.000000 zenaura-0.9.96/tests/test_rdom_adapter.py
--rw-rw-rw-   0        0        0     1201 2024-05-27 20:12:21.000000 zenaura-0.9.96/tests/test_server.py
--rw-rw-rw-   0        0        0    15215 2024-05-26 17:44:57.000000 zenaura-0.9.96/tests/test_tags.py
--rw-rw-rw-   0        0        0     3293 2024-05-26 17:44:57.000000 zenaura-0.9.96/tests/test_tasker.py
--rw-rw-rw-   0        0        0     5456 2024-05-26 17:44:57.000000 zenaura-0.9.96/tests/test_zenaura_dom.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:46:28.555752 zenaura-0.9.96/zenaura/
--rw-rw-rw-   0        0        0        0 2024-05-26 19:08:09.000000 zenaura-0.9.96/zenaura/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:46:28.568753 zenaura-0.9.96/zenaura/client/
--rw-rw-rw-   0        0        0        0 2024-05-26 18:57:31.000000 zenaura-0.9.96/zenaura/client/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:46:28.572252 zenaura-0.9.96/zenaura/client/algorithm/
--rw-rw-rw-   0        0        0       39 2024-05-26 17:44:57.000000 zenaura-0.9.96/zenaura/client/algorithm/__init__.py
--rw-rw-rw-   0        0        0      193 2024-05-26 17:44:57.000000 zenaura-0.9.96/zenaura/client/algorithm/algorithm.py
--rw-rw-rw-   0        0        0      972 2024-05-26 17:44:57.000000 zenaura-0.9.96/zenaura/client/algorithm/operations.py
--rw-rw-rw-   0        0        0     7166 2024-05-26 18:57:08.000000 zenaura-0.9.96/zenaura/client/algorithm/searcher.py
--rw-rw-rw-   0        0        0     2772 2024-05-26 18:57:08.000000 zenaura-0.9.96/zenaura/client/algorithm/updater.py
--rw-rw-rw-   0        0        0    10510 2024-05-27 23:18:46.000000 zenaura-0.9.96/zenaura/client/app.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:46:28.574253 zenaura-0.9.96/zenaura/client/compiler/
--rw-rw-rw-   0        0        0       53 2024-05-26 17:44:57.000000 zenaura-0.9.96/zenaura/client/compiler/__init__.py
--rw-rw-rw-   0        0        0     1403 2024-05-26 18:57:08.000000 zenaura-0.9.96/zenaura/client/compiler/attribute.py
--rw-rw-rw-   0        0        0     3471 2024-05-26 18:57:08.000000 zenaura-0.9.96/zenaura/client/compiler/compiler.py
--rw-rw-rw-   0        0        0     1132 2024-05-26 17:44:57.000000 zenaura-0.9.96/zenaura/client/compiler/sanitize.py
--rw-rw-rw-   0        0        0     4093 2024-05-26 18:57:08.000000 zenaura-0.9.96/zenaura/client/component.py
--rw-rw-rw-   0        0        0      744 2024-05-26 17:44:57.000000 zenaura-0.9.96/zenaura/client/config.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:46:28.577259 zenaura-0.9.96/zenaura/client/dom/
--rw-rw-rw-   0        0        0       43 2024-05-26 17:44:57.000000 zenaura-0.9.96/zenaura/client/dom/__init__.py
--rw-rw-rw-   0        0        0      280 2024-05-26 17:44:57.000000 zenaura-0.9.96/zenaura/client/dom/dom.py
--rw-rw-rw-   0        0        0     1803 2024-05-26 18:57:08.000000 zenaura-0.9.96/zenaura/client/dom/error.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:46:28.578264 zenaura-0.9.96/zenaura/client/dom/lifecycles/
--rw-rw-rw-   0        0        0      449 2024-05-27 19:25:39.000000 zenaura-0.9.96/zenaura/client/dom/lifecycles/mount.py
--rw-rw-rw-   0        0        0      804 2024-05-27 19:26:03.000000 zenaura-0.9.96/zenaura/client/dom/lifecycles/render.py
--rw-rw-rw-   0        0        0     1488 2024-05-29 18:48:04.000000 zenaura-0.9.96/zenaura/client/dom/mount.py
--rw-rw-rw-   0        0        0     1895 2024-05-27 20:46:41.000000 zenaura-0.9.96/zenaura/client/dom/render.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:46:28.582265 zenaura-0.9.96/zenaura/client/hydrator/
--rw-rw-rw-   0        0        0      235 2024-05-26 17:44:57.000000 zenaura-0.9.96/zenaura/client/hydrator/__init__.py
--rw-rw-rw-   0        0        0     1895 2024-05-26 18:57:08.000000 zenaura-0.9.96/zenaura/client/hydrator/compiler_adapter.py
--rw-rw-rw-   0        0        0     1236 2024-05-26 17:44:57.000000 zenaura-0.9.96/zenaura/client/hydrator/hydrator.py
--rw-rw-rw-   0        0        0     1346 2024-05-26 17:44:57.000000 zenaura-0.9.96/zenaura/client/hydrator/lookup.py
--rw-rw-rw-   0        0        0     7033 2024-05-27 22:07:22.000000 zenaura-0.9.96/zenaura/client/hydrator/real_dom_adapter.py
--rw-rw-rw-   0        0        0     2264 2024-05-26 17:44:57.000000 zenaura-0.9.96/zenaura/client/hydrator/tasker.py
--rw-rw-rw-   0        0        0     1064 2024-05-26 18:57:08.000000 zenaura-0.9.96/zenaura/client/hydrator/virtual_dom_adapter.py
--rw-rw-rw-   0        0        0     2631 2024-05-26 17:44:57.000000 zenaura-0.9.96/zenaura/client/mocks.py
--rw-rw-rw-   0        0        0      896 2024-05-26 18:57:08.000000 zenaura-0.9.96/zenaura/client/mutator.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:46:28.584265 zenaura-0.9.96/zenaura/client/observer/
--rw-rw-rw-   0        0        0       60 2024-05-26 17:44:57.000000 zenaura-0.9.96/zenaura/client/observer/__init__.py
--rw-rw-rw-   0        0        0      396 2024-05-26 17:44:57.000000 zenaura-0.9.96/zenaura/client/observer/observer.py
--rw-rw-rw-   0        0        0     1609 2024-05-26 17:44:57.000000 zenaura-0.9.96/zenaura/client/observer/subject.py
--rw-rw-rw-   0        0        0     2009 2024-05-26 17:44:57.000000 zenaura-0.9.96/zenaura/client/observer.py
--rw-rw-rw-   0        0        0      735 2024-05-27 20:29:15.000000 zenaura-0.9.96/zenaura/client/page.py
--rw-rw-rw-   0        0        0     2212 2024-05-26 17:44:57.000000 zenaura-0.9.96/zenaura/client/persistance.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:46:28.587737 zenaura-0.9.96/zenaura/client/tags/
--rw-rw-rw-   0        0        0      165 2024-05-26 17:44:57.000000 zenaura-0.9.96/zenaura/client/tags/__init__.py
--rw-rw-rw-   0        0        0      429 2024-05-26 17:44:57.000000 zenaura-0.9.96/zenaura/client/tags/attribute.py
--rw-rw-rw-   0        0        0     4666 2024-05-26 17:44:57.000000 zenaura-0.9.96/zenaura/client/tags/builder.py
--rw-rw-rw-   0        0        0      418 2024-05-26 17:44:57.000000 zenaura-0.9.96/zenaura/client/tags/data.py
--rw-rw-rw-   0        0        0      473 2024-05-26 17:44:57.000000 zenaura-0.9.96/zenaura/client/tags/html.py
--rw-rw-rw-   0        0        0    10231 2024-05-26 17:44:57.000000 zenaura-0.9.96/zenaura/client/tags/node.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:46:28.589237 zenaura-0.9.96/zenaura/server/
--rw-rw-rw-   0        0        0       33 2024-05-26 19:08:17.000000 zenaura-0.9.96/zenaura/server/__init__.py
--rw-rw-rw-   0        0        0     3531 2024-05-30 13:45:40.000000 zenaura-0.9.96/zenaura/server/server.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:46:28.589737 zenaura-0.9.96/zenaura.egg-info/
--rw-rw-rw-   0        0        0     2028 2024-05-30 13:46:28.000000 zenaura-0.9.96/zenaura.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1888 2024-05-30 13:46:28.000000 zenaura-0.9.96/zenaura.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 13:46:28.000000 zenaura-0.9.96/zenaura.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-30 13:46:28.000000 zenaura-0.9.96/zenaura.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-30 13:46:28.000000 zenaura-0.9.96/zenaura.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 17:55:36.465055 zenaura-0.9.97/
+-rw-rw-rw-   0        0        0     1100 2024-05-11 11:29:30.000000 zenaura-0.9.97/LICENSE
+-rw-rw-rw-   0        0        0     2028 2024-06-01 17:55:36.464556 zenaura-0.9.97/PKG-INFO
+-rw-rw-rw-   0        0        0     1376 2024-05-26 16:54:28.000000 zenaura-0.9.97/README.md
+-rw-rw-rw-   0        0        0       42 2024-06-01 17:55:36.465055 zenaura-0.9.97/setup.cfg
+-rw-rw-rw-   0        0        0     1135 2024-06-01 17:55:10.000000 zenaura-0.9.97/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 17:55:36.423051 zenaura-0.9.97/tests/
+-rw-rw-rw-   0        0        0    33440 2024-05-26 17:44:57.000000 zenaura-0.9.97/tests/test_algorithm.py
+-rw-rw-rw-   0        0        0     6595 2024-05-27 20:30:05.000000 zenaura-0.9.97/tests/test_app.py
+-rw-rw-rw-   0        0        0     7595 2024-05-26 17:44:57.000000 zenaura-0.9.97/tests/test_compiler.py
+-rw-rw-rw-   0        0        0     4161 2024-05-26 17:44:57.000000 zenaura-0.9.97/tests/test_component_e2e.py
+-rw-rw-rw-   0        0        0     1415 2024-05-26 17:44:57.000000 zenaura-0.9.97/tests/test_component_unit.py
+-rw-rw-rw-   0        0        0     5301 2024-05-26 17:44:57.000000 zenaura-0.9.97/tests/test_node_properties.py
+-rw-rw-rw-   0        0        0     1435 2024-05-26 17:44:57.000000 zenaura-0.9.97/tests/test_observer.py
+-rw-rw-rw-   0        0        0     5710 2024-05-26 17:44:57.000000 zenaura-0.9.97/tests/test_rdom_adapter.py
+-rw-rw-rw-   0        0        0     1201 2024-05-27 20:12:21.000000 zenaura-0.9.97/tests/test_server.py
+-rw-rw-rw-   0        0        0    15215 2024-05-26 17:44:57.000000 zenaura-0.9.97/tests/test_tags.py
+-rw-rw-rw-   0        0        0     3293 2024-05-26 17:44:57.000000 zenaura-0.9.97/tests/test_tasker.py
+-rw-rw-rw-   0        0        0     5456 2024-05-26 17:44:57.000000 zenaura-0.9.97/tests/test_zenaura_dom.py
+drwxrwxrwx   0        0        0        0 2024-06-01 17:55:36.423550 zenaura-0.9.97/zenaura/
+-rw-rw-rw-   0        0        0        0 2024-05-26 19:08:09.000000 zenaura-0.9.97/zenaura/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 17:55:36.436052 zenaura-0.9.97/zenaura/client/
+-rw-rw-rw-   0        0        0        0 2024-05-26 18:57:31.000000 zenaura-0.9.97/zenaura/client/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 17:55:36.439052 zenaura-0.9.97/zenaura/client/algorithm/
+-rw-rw-rw-   0        0        0       39 2024-05-26 17:44:57.000000 zenaura-0.9.97/zenaura/client/algorithm/__init__.py
+-rw-rw-rw-   0        0        0     1516 2024-05-30 17:33:35.000000 zenaura-0.9.97/zenaura/client/algorithm/algorithm.py
+-rw-rw-rw-   0        0        0      972 2024-05-26 17:44:57.000000 zenaura-0.9.97/zenaura/client/algorithm/operations.py
+-rw-rw-rw-   0        0        0     9510 2024-05-30 18:06:30.000000 zenaura-0.9.97/zenaura/client/algorithm/searcher.py
+-rw-rw-rw-   0        0        0     4602 2024-05-30 17:50:50.000000 zenaura-0.9.97/zenaura/client/algorithm/updater.py
+-rw-rw-rw-   0        0        0    11549 2024-05-30 18:20:25.000000 zenaura-0.9.97/zenaura/client/app.py
+drwxrwxrwx   0        0        0        0 2024-06-01 17:55:36.440552 zenaura-0.9.97/zenaura/client/compiler/
+-rw-rw-rw-   0        0        0       53 2024-05-26 17:44:57.000000 zenaura-0.9.97/zenaura/client/compiler/__init__.py
+-rw-rw-rw-   0        0        0     1995 2024-05-30 17:53:18.000000 zenaura-0.9.97/zenaura/client/compiler/attribute.py
+-rw-rw-rw-   0        0        0     4304 2024-05-30 18:06:35.000000 zenaura-0.9.97/zenaura/client/compiler/compiler.py
+-rw-rw-rw-   0        0        0     1821 2024-05-30 17:55:09.000000 zenaura-0.9.97/zenaura/client/compiler/sanitize.py
+-rw-rw-rw-   0        0        0     6018 2024-05-30 18:21:42.000000 zenaura-0.9.97/zenaura/client/component.py
+-rw-rw-rw-   0        0        0      744 2024-05-26 17:44:57.000000 zenaura-0.9.97/zenaura/client/config.py
+drwxrwxrwx   0        0        0        0 2024-06-01 17:55:36.443050 zenaura-0.9.97/zenaura/client/dom/
+-rw-rw-rw-   0        0        0       43 2024-05-26 17:44:57.000000 zenaura-0.9.97/zenaura/client/dom/__init__.py
+-rw-rw-rw-   0        0        0     1243 2024-05-30 17:57:32.000000 zenaura-0.9.97/zenaura/client/dom/dom.py
+-rw-rw-rw-   0        0        0     2969 2024-05-30 17:58:34.000000 zenaura-0.9.97/zenaura/client/dom/error.py
+drwxrwxrwx   0        0        0        0 2024-06-01 17:55:36.444551 zenaura-0.9.97/zenaura/client/dom/lifecycles/
+-rw-rw-rw-   0        0        0      930 2024-05-30 17:56:03.000000 zenaura-0.9.97/zenaura/client/dom/lifecycles/mount.py
+-rw-rw-rw-   0        0        0     1557 2024-05-30 17:56:46.000000 zenaura-0.9.97/zenaura/client/dom/lifecycles/render.py
+-rw-rw-rw-   0        0        0     2700 2024-05-30 17:59:41.000000 zenaura-0.9.97/zenaura/client/dom/mount.py
+-rw-rw-rw-   0        0        0     4547 2024-05-30 18:01:23.000000 zenaura-0.9.97/zenaura/client/dom/render.py
+drwxrwxrwx   0        0        0        0 2024-06-01 17:55:36.448051 zenaura-0.9.97/zenaura/client/hydrator/
+-rw-rw-rw-   0        0        0      235 2024-05-26 17:44:57.000000 zenaura-0.9.97/zenaura/client/hydrator/__init__.py
+-rw-rw-rw-   0        0        0     2041 2024-05-30 17:37:43.000000 zenaura-0.9.97/zenaura/client/hydrator/compiler_adapter.py
+-rw-rw-rw-   0        0        0     1193 2024-05-30 17:38:53.000000 zenaura-0.9.97/zenaura/client/hydrator/hydrator.py
+-rw-rw-rw-   0        0        0     1376 2024-05-30 17:39:44.000000 zenaura-0.9.97/zenaura/client/hydrator/lookup.py
+-rw-rw-rw-   0        0        0     8918 2024-05-30 17:45:58.000000 zenaura-0.9.97/zenaura/client/hydrator/real_dom_adapter.py
+-rw-rw-rw-   0        0        0     3441 2024-05-30 17:47:33.000000 zenaura-0.9.97/zenaura/client/hydrator/tasker.py
+-rw-rw-rw-   0        0        0     1064 2024-05-26 18:57:08.000000 zenaura-0.9.97/zenaura/client/hydrator/virtual_dom_adapter.py
+-rw-rw-rw-   0        0        0     7226 2024-05-30 18:23:13.000000 zenaura-0.9.97/zenaura/client/mocks.py
+-rw-rw-rw-   0        0        0     1223 2024-05-30 18:24:01.000000 zenaura-0.9.97/zenaura/client/mutator.py
+drwxrwxrwx   0        0        0        0 2024-06-01 17:55:36.449550 zenaura-0.9.97/zenaura/client/observer/
+-rw-rw-rw-   0        0        0       60 2024-05-26 17:44:57.000000 zenaura-0.9.97/zenaura/client/observer/__init__.py
+-rw-rw-rw-   0        0        0     2674 2024-05-30 18:02:13.000000 zenaura-0.9.97/zenaura/client/observer/observer.py
+-rw-rw-rw-   0        0        0     3384 2024-05-30 18:03:02.000000 zenaura-0.9.97/zenaura/client/observer/subject.py
+-rw-rw-rw-   0        0        0     1346 2024-05-30 18:25:55.000000 zenaura-0.9.97/zenaura/client/page.py
+-rw-rw-rw-   0        0        0     4235 2024-05-30 18:26:50.000000 zenaura-0.9.97/zenaura/client/persistance.py
+drwxrwxrwx   0        0        0        0 2024-06-01 17:55:36.452551 zenaura-0.9.97/zenaura/client/tags/
+-rw-rw-rw-   0        0        0      141 2024-05-30 18:06:40.000000 zenaura-0.9.97/zenaura/client/tags/__init__.py
+-rw-rw-rw-   0        0        0      925 2024-05-30 18:04:18.000000 zenaura-0.9.97/zenaura/client/tags/attribute.py
+-rw-rw-rw-   0        0        0     5021 2024-05-30 18:05:15.000000 zenaura-0.9.97/zenaura/client/tags/builder.py
+-rw-rw-rw-   0        0        0     1325 2024-05-30 18:08:24.000000 zenaura-0.9.97/zenaura/client/tags/html.py
+-rw-rw-rw-   0        0        0    11710 2024-05-30 18:13:18.000000 zenaura-0.9.97/zenaura/client/tags/node.py
+drwxrwxrwx   0        0        0        0 2024-06-01 17:55:36.463055 zenaura-0.9.97/zenaura/server/
+-rw-rw-rw-   0        0        0       33 2024-05-26 19:08:17.000000 zenaura-0.9.97/zenaura/server/__init__.py
+-rw-rw-rw-   0        0        0    12254 2024-06-01 17:54:54.000000 zenaura-0.9.97/zenaura/server/server.py
+drwxrwxrwx   0        0        0        0 2024-06-01 17:55:36.464055 zenaura-0.9.97/zenaura.egg-info/
+-rw-rw-rw-   0        0        0     2028 2024-06-01 17:55:36.000000 zenaura-0.9.97/zenaura.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1833 2024-06-01 17:55:36.000000 zenaura-0.9.97/zenaura.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 17:55:36.000000 zenaura-0.9.97/zenaura.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-06-01 17:55:36.000000 zenaura-0.9.97/zenaura.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-06-01 17:55:36.000000 zenaura-0.9.97/zenaura.egg-info/top_level.txt
```

### Comparing `zenaura-0.9.96/LICENSE` & `zenaura-0.9.97/LICENSE`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.96/PKG-INFO` & `zenaura-0.9.97/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zenaura
-Version: 0.9.96
+Version: 0.9.97
 Summary: Zenaura is an experimental Python library built upon PyScript, designed to empower Python developers to create stateful, component-based Single Page Applications (SPAs). By leveraging a virtual DOM implementation, Zenaura optimizes the performance, reactivity, responsiveness, and interactivity of web applications. This allows developers to build high-performance, dynamic web applications using familiar Python concepts and syntax.
 Author: Ahmed Rakan
 Author-email: ar.aldhafeeri11@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bleach
```

### Comparing `zenaura-0.9.96/README.md` & `zenaura-0.9.97/README.md`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.96/setup.py` & `zenaura-0.9.97/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='zenaura',
-    version='0.9.96',
+    version='0.9.97',
     description="Zenaura is an experimental Python library built upon PyScript, designed to empower Python developers to create stateful, component-based Single Page Applications (SPAs). By leveraging a virtual DOM implementation, Zenaura optimizes the performance, reactivity, responsiveness, and interactivity of web applications. This allows developers to build high-performance, dynamic web applications using familiar Python concepts and syntax.",
     author="Ahmed Rakan",
     author_email="ar.aldhafeeri11@gmail.com",
     packages=['zenaura', 'zenaura.server', 'zenaura.client', 'zenaura.client.algorithm', 'zenaura.client.compiler', 'zenaura.client.hydrator', 'zenaura.client.observer', 'zenaura.client.tags', 'zenaura.client.dom', 'zenaura.client.dom.lifecycles'],
     install_requires=[
         'bleach'
     ],
```

### Comparing `zenaura-0.9.96/tests/test_algorithm.py` & `zenaura-0.9.97/tests/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.96/tests/test_app.py` & `zenaura-0.9.97/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.96/tests/test_compiler.py` & `zenaura-0.9.97/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.96/tests/test_component_e2e.py` & `zenaura-0.9.97/tests/test_component_e2e.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.96/tests/test_component_unit.py` & `zenaura-0.9.97/tests/test_component_unit.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.96/tests/test_node_properties.py` & `zenaura-0.9.97/tests/test_node_properties.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.96/tests/test_observer.py` & `zenaura-0.9.97/tests/test_observer.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.96/tests/test_rdom_adapter.py` & `zenaura-0.9.97/tests/test_rdom_adapter.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.96/tests/test_server.py` & `zenaura-0.9.97/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.96/tests/test_tags.py` & `zenaura-0.9.97/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.96/tests/test_tasker.py` & `zenaura-0.9.97/tests/test_tasker.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.96/tests/test_zenaura_dom.py` & `zenaura-0.9.97/tests/test_zenaura_dom.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.96/zenaura/client/algorithm/operations.py` & `zenaura-0.9.97/zenaura/client/algorithm/operations.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.96/zenaura/client/app.py` & `zenaura-0.9.97/zenaura/client/app.py`

 * *Files 13% similar despite different names*

```diff
@@ -79,47 +79,56 @@
             The title of the route.
         path : str
             The path of the route.
         page : Page
             A page of pageonents.
         handler : Optional[Callable]
             Optional route-specific logic handler.
+        middleware : Optional[Callable]
+            Optional route-specific logic handler.
+        ssr : bool
+            Whether the route is server-side rendered.
         """
         self.title = title
         self.path = path
         self.page = page
         self.ssr=ssr
 
         if not isinstance(page, Page):
             raise TypeError("Only a Page can be mounted on a route")
         self.middleware: Optional[Callable] = middleware  # For optional route-specific logic
 
 
 # router 
 class App:
     """
-        Represents a router for managing routes and navigation.
+    Represents a router for managing routes and navigation.
+
+    This class provides methods for adding routes, navigating between pages, and handling the current location.
 
-        Methods
-        -------
+    Attributes:
+        routes (dict): A dictionary mapping paths to their associated pages and titles.
+        paths (list): A list of paths registered in the router.
+        history (PageHistory): An object that manages the history of visited pages.
+
+    Methods:
         __init__()
             Initializes the App with empty routes and paths, and sets up the initial route handling.
         navigate(path)
-            Navigates to the specified path by mounting the associated pageonent and updating the document title and browser history.
+            Navigates to the specified path by mounting the associated page and updating the document title and browser history.
         handle_location()
-            Handles the current location by mounting the associated pageonent and updating the document title.
+            Handles the current location by mounting the associated page and updating the document title.
         add_route(route)
             Adds a route to the router's configuration.
-
-        Attributes
-        ----------
-        routes : dict
-            A dictionary mapping paths to their associated pageonents and titles.
-        paths : list
-            A list of paths registered in the router.
+        back()
+            Navigates back to the previous Page in the history stack.
+        forward()
+            Navigates forward to the next Page in the history stack.
+        get_current_route()
+            Get the page and title of the current route, or None if not found.
     """
     def __init__(self):
         """
             Initializes the App with empty routes and paths, and sets up the initial route handling.
         """
         # key -> path , value -> [page, document.title]
         self.routes = defaultdict(str)
@@ -211,40 +220,57 @@
         route : Route
             The route to be added to the router's configuration.
         """
         self.routes[route.path] = [route.page, route.title, route.middleware, route.ssr]
         self.paths.append(route.path)
     
     async def back(self) -> None:
+        """
+        Navigates back to the previous Page in the history stack.
+        """
         previous_page = self.history.current.page
         curr_page = self.history.back()
         if not curr_page.ssr: # ignore mount step for server side rendering pages.
             rdom_hyd.hyd_rdom_toggle_pages_visibilty(previous_page, curr_page)
             await zenaura_dom.mount(curr_page)  # trigger attached lifecycle for each component within the page.
         else: # trigger attached lifecycle method for the component.
             await zenaura_dom.mount(curr_page)
     
     async def forward(self) -> None:
+        """
+        Navigates forward to the next Page in the history stack.
+        """
         previous_page = self.history.current.page
         curr_page = self.history.forward()
         if not curr_page.ssr: # ignore mount step for server side rendering pages.
             rdom_hyd.hyd_rdom_toggle_pages_visibilty(previous_page, curr_page)
             await zenaura_dom.mount(curr_page)  # trigger attached lifecycle for each component within the page.
         else: # trigger attached lifecycle method for the component.
             await zenaura_dom.mount(curr_page)
 
     def get_current_route(self) -> Optional[Tuple[Page, str]]:
-            """Get the page and title of the current route, or None if not found."""
-            path = window.location.pathname
-            matched_route, info = self._match_route(path)
-            return matched_route, info
+        """
+        Get the page and title of the current route, or None if not found.
+        """
+        path = window.location.pathname
+        matched_route, info = self._match_route(path)
+        return matched_route, info
     
     # TODO still needs a lot of work
     def _match_route(self, path: str) -> Tuple[Optional[Tuple[Page, str, Dict[str, Any]]], Dict[str, str]]:
-        """Matches the given path to a registered route and extracts parameters."""
+        """
+        Matches the given path to a registered route and extracts parameters.
+
+        Args:
+            path (str): The path to match.
+
+        Returns:
+            Tuple[Optional[Tuple[Page, str, Dict[str, Any]]], Dict[str, str]]:
+                A tuple containing the matched route information (if any) and extracted parameters.
+        """
         for route_path, (page, title, middleware, ssr) in self.routes.items():
             if "*" in route_path:  # Wildcard route
                 route_parts = route_path.split("*")
                 if path.startswith(route_parts[0]):
                     params = path[len(route_parts[0]):]
                     query = defaultdict(str)
                     if "?" in params: # get all queries
```

### Comparing `zenaura-0.9.96/zenaura/client/compiler/attribute.py` & `zenaura-0.9.97/zenaura/client/compiler/attribute.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,48 @@
 from zenaura.client.tags import Attribute
 from .sanitize import CompilerSanitizer
 from typing import List 
 import io 
 
 sanitizer = CompilerSanitizer()
+
 class AttributeProccessor(
+    ):
+    """
+    This class is responsible for processing a list of `Attribute` objects and converting them into HTML-formatted attributes.
+
+    Attributes:
+        None
+    """
 
-):
     def process_attributes(
                 self, 
                 attrs: List[Attribute]
                 ) -> str:
         """
-            Processes a list of Attributes, converting them to
-            HTML-formatted attributes.
+        Processes a list of `Attribute` objects, converting them to HTML-formatted attributes.
+
+        Args:
+            attrs (List[Attribute]): A list of `Attribute` objects representing the attributes to be processed.
+
+        Returns:
+            str: A string containing the HTML-formatted attributes, ready to be included in a tag.
 
-            Args:
-                attrs (List[Attribute]): A list of Zenui Attribute objects.
-                attributes like onclick.
-
-            Returns:
-                str: A string containing the HTML-formatted attributes,
-                 ready to be included in a tag.
+        Raises:
+            TypeError: If the input `attrs` is not a list.
+            ValueError: If any element in `attrs` is not an `Attribute` object.
         """
 
+        if not isinstance(attrs, list):
+            raise TypeError("`attrs` must be a list of Attribute objects.")
+
+        for attr in attrs:
+            if not isinstance(attr, Attribute):
+                raise ValueError("Each element in `attrs` must be an Attribute object.")
+
         s = io.StringIO()  # Create a string buffer for building the output
 
         for i, attr in enumerate(attrs):
             attrKey = attr.key
             attrValue = attr.value
             if attrKey in self.attrKeyWords.keys():
                 attrKey = self.attrKeyWords[attrKey]  # Apply keyword mapping
@@ -36,8 +51,8 @@
             if i == 0 or i == len(attrs) - 1:
                 s.write(f' {attrKey}="{sanitizer.sanitize(attrValue)}"')
             else:
                 s.write(f'{attrKey}="{sanitizer.sanitize(attrValue)}" ')
 
         res = s.getvalue()
         s.close()
-        return res
+        return res
```

### Comparing `zenaura-0.9.96/zenaura/client/component.py` & `zenaura-0.9.97/zenaura/client/component.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,26 +14,43 @@
         # Combine class name and count to create a unique string
         unique_string = f"{cls_name}{count}"
         # Hash the unique string to produce a 32-bit UUID
         uuid_hash = hashlib.md5(unique_string.encode()).hexdigest()[:8]
         return uuid_hash
 
 def Reuseable(cls):
+    """
+    Decorator to mark a component as reusable.
+
+    Reusable components can be instantiated multiple times and will maintain their own state.
+
+    Args:
+        cls (type): The component class to be decorated.
+
+    Returns:
+        type: The decorated component class.
+    """
+
     original_init = cls.__init__
 
     def new_init(self, *args, **kwargs):
         original_init(self, *args, **kwargs)
         cls.count = next(cls._component_count)
         self.id = UUIDManager.generate_uuid(cls.__name__, self.count)
         _is_reuseable[cls.__name__] = True
 
     cls.__init__ = new_init
     return cls
 
 class SelectiveSingleton(type):
+    """
+    Metaclass to ensure only one instance of a component exists at a time.
+
+    This metaclass is used for components that should only have one instance, even if they are instantiated multiple times.
+    """
     _instances = defaultdict(str)
 
     def __call__(cls, *args, **kwargs):
         # Check if the class has the _is_reuseable attribute set to True
         if not _is_reuseable[cls.__name__]:
             return super().__call__(*args, **kwargs)
 
@@ -43,24 +60,55 @@
             cls._instances[cls] = instance
         else:
             instance = super().__call__(*args, **kwargs)
             cls._instances[reuseableId] = instance
         return cls._instances[cls]
     
 class Component(metaclass=SelectiveSingleton):
+    """
+    Base class for all Zenaura components.
+
+    Components are the building blocks of Zenaura applications. They represent reusable units of functionality that can be composed to create complex user interfaces.
+
+    Attributes:
+        id (str): A unique identifier for the component.
+        state (dict): The state of the component.
+        _state (dict): The internal state of the component.
+        _track_instances (dict): A dictionary tracking the number of instances created for each component class.
+        _component_count (itertools.count): An iterator that generates unique counts for each component instance.
+
+    Methods:
+        __init_subclass__(cls, **kwargs):
+            Initializes the subclass and sets the initial count for the component class.
+        __init__(self):
+            Initializes the component instance and sets the unique identifier.
+        get_state(self):
+            Returns the state of the component.
+        set_state(self, state):
+            Sets the state of the component.
+        render(self):
+            Abstract method that must be implemented by subclasses to define the behavior of the component.
+    """
+
     _state = defaultdict(str)
     _track_instances = defaultdict(int)
     _component_count = itertools.count(0)
 
     def __init_subclass__(cls, **kwargs):
+        """
+        Initializes the subclass and sets the initial count for the component class.
+        """
         cls.count = next(cls._component_count)
         cls.id = UUIDManager.generate_uuid(cls.__name__, cls.count)
         super().__init_subclass__(**kwargs)
         
     def __init__(self):
+        """
+        Initializes the component instance and sets the unique identifier.
+        """
         cls = self.__class__
         Component._track_instances[cls.__name__] += 1
         if Component._track_instances[cls.__name__] > 1 and not _is_reuseable[cls.__name__]:
             raise TypeError(
 """
     Zenaura class component are limted by design. \n
     Decorate component with @Reuseable to implicitly  \n
```

### Comparing `zenaura-0.9.96/zenaura/client/config.py` & `zenaura-0.9.97/zenaura/client/config.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.96/zenaura/client/dom/lifecycles/render.py` & `zenaura-0.9.97/zenaura/client/dom/lifecycles/mount.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,31 @@
-class RenderLifeCycle:
-    async def on_mutation(self, comp) -> None:
-        """
-        Method called after the component is updated in the DOM and re-rendered.
+from zenaura.client.hydrator import HydratorVirtualDomAdapter
 
-        Parameters:
-        - comp: An instance of the Component class.
+class MountLifeCycles(
+    HydratorVirtualDomAdapter
+):
+    """
+    This class provides lifecycle methods for components that are mounted to the DOM.
 
-        Returns:
-        None
-        """
-        # Perform operations before updating
-        if hasattr(comp, 'on_mutation'):
-            await comp.on_mutation()
+    It inherits from the `HydratorVirtualDomAdapter` class, which provides methods for interacting with the virtual DOM.
+    """
 
-    async def on_settled(self, comp) -> None:
+    async def attached(self, comp) -> None:
         """
-        Method called after the component is updated in the DOM and re-rendered.
+        This method is called after the component is mounted to the DOM.
 
-        Parameters:
-        - comp: An instance of the Component class.
+        It allows the component to perform any necessary actions after it has been added to the DOM, such as:
+
+        - Initializing state
+        - Setting up event listeners
+        - Making API calls
+        - Performing animations
+
+        Args:
+            comp: An instance of the Component class.
 
         Returns:
-        None
+            None
         """
-        # Perform operations after updating
-        if hasattr(comp, 'on_settled'):
-            await comp.on_settled()
+
+        if hasattr(comp, 'attached'):
+            await comp.attached()
```

### Comparing `zenaura-0.9.96/zenaura/client/hydrator/compiler_adapter.py` & `zenaura-0.9.97/zenaura/client/hydrator/compiler_adapter.py`

 * *Files 11% similar despite different names*

```diff
@@ -53,14 +53,18 @@
         return compiler.compile(
             children, 
             id=id,
             zenaura_dom_mode=True,
         )
     
     def hyd_comp_compile_page(self, page: Page) -> str:
+        """
+            compiler operation : wraps compiler compile, returns str "HTMLElement"
+            compiles page children
+        """
         html = io.StringIO()
         for comp in page.children:
             html.write(
                 compiler.compile(
                     comp.render(), 
                     comp.id,
                     zenaura_dom_mode=True,
```

### Comparing `zenaura-0.9.96/zenaura/client/hydrator/hydrator.py` & `zenaura-0.9.97/zenaura/client/hydrator/hydrator.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,33 +9,20 @@
 class Hydrator(
     HydratorVirtualDomAdapter,
     HydratorCompilerAdapter,
     HydratorRealDomAdapter,
     HydratorTasker
 ):
     """
-        Hydrator is the bridge of communication between:
-        1. Virtual dom and compiler :
-            methods that communicate with the compiler
-            should start with:
-            hyd_comp_
-            e.g. :
-            hyd_comp_get_keyed_uuid
-            hyd_comp_compile_node
-        2. Virtual dom : 
-            methods that interact with zenaura virtual dom.
-            should start with:
-            hyd_vdom_
-            e.g. :
-            hyd_vdom_update
-            hyd_vdom_delete
-        3. DOM : 
-            methods that interact with the DOM.
-            should start with:
-            hyd_dom_
-            e.g. :
-            hyd_rdom_attach_to_root
-        4. Tasker:
-            task to update the dom are created in the updeter.
-            dequeued in render lifecycle and 
-            updates the dom asynchronously
+    Hydrator acts as the central communication hub between:
+
+    1. **Virtual DOM and Compiler:**
+        - Methods interacting with the compiler start with `hyd_comp_`, e.g., `hyd_comp_get_keyed_uuid`, `hyd_comp_compile_node`.
+    2. **Virtual DOM:**
+        - Methods interacting with Zenaura's virtual DOM start with `hyd_vdom_`, e.g., `hyd_vdom_update`, `hyd_vdom_delete`.
+    3. **DOM:**
+        - Methods interacting with the DOM start with `hyd_dom_`, e.g., `hyd_rdom_attach_to_root`.
+    4. **Tasker:**
+        - Tasks for updating the DOM are created in the updater and dequeued during the render lifecycle, enabling asynchronous DOM updates.
+
+    Essentially, Hydrator bridges the gap between various components within the Zenaura framework, facilitating seamless communication and efficient DOM manipulation.
     """
```

### Comparing `zenaura-0.9.96/zenaura/client/hydrator/lookup.py` & `zenaura-0.9.97/zenaura/client/hydrator/lookup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 from collections import defaultdict
 
 class VDomLookupTable:
     """
-        1. zen_dom_table :
-        - Optimizing general tree structure
-        - each component unique id
-        - each child of the component has ZENAURA_DOM_ATTRIBUTE
-        this allows for:
-        - searching for mounted component prev state : O(1)
-        - deleting unmounted components : O(1)
-        - inserting mounted components : O(1)
-        now same time complexity applies on tree structure:
-        - search O(n)
-        - insert O(n)
-        - delete O(n)
-        - update O(n)
-        aslo allows for effecient management of memory
-        since in zenaura one page and each page is a dummy node
-        of children components
-        then once the page unmounted all the components are deleted
+        VDomLookupTable:
 
-        2. zenaura prev_page_instance:
-        - once page is mounted we store the prev_page_instance
-        - zenaura mount single page at a time or " route path "
-        - this allow for effecient memory management
-        - once new page is mounted:
-            - get the prev page instance
-            - iterage over the prev page components
-            - delete the prev page component from zen_dom_table
+        This class manages two lookup tables:
+
+        1. **zen_dom_table**:
+            - Optimizes general tree structure by storing each component's unique ID and its children with the `ZENAURA_DOM_ATTRIBUTE`.
+            - Provides efficient operations:
+                - Searching for mounted component's previous state: O(1)
+                - Deleting unmounted components: O(1)
+                - Inserting mounted components: O(1)
+            - Applies the same time complexity to tree structure operations:
+                - Search: O(n)
+                - Insert: O(n)
+                - Delete: O(n)
+                - Update: O(n)
+            - Enables efficient memory management by deleting all components when a page is unmounted.
+
+        2. **zenaura_prev_page_instance**:
+            - Stores the previously mounted page instance.
+            - Leverages Zenaura's single-page mounting (per route path) for efficient memory management.
+            - When a new page is mounted:
+                - Retrieves the previous page instance.
+                - Iterates over its components and deletes them from `zen_dom_table`.
 
     """
     zen_dom_table = defaultdict(str)
     prev_page_instance = None
     zen_pre_compiled = defaultdict(str)
```

### Comparing `zenaura-0.9.96/zenaura/client/hydrator/real_dom_adapter.py` & `zenaura-0.9.97/zenaura/client/hydrator/real_dom_adapter.py`

 * *Files 22% similar despite different names*

```diff
@@ -23,38 +23,46 @@
         methods should start with:
         hyd_romp_
     """
 
 
     def hyd_rdom_create_element(self, virtual_node: Node) -> HTMLElement:
         """
-            DOM operation : creates html element and returns it as HTMLElement
+        DOM operation: creates html element and returns it as HTMLElement
+
+        Args:
+            virtual_node: Node - the virtual node representing the element to be created
+
+        Returns:
+            HTMLElement - the created HTML element
         """
         element = document.createElement(virtual_node.name)
         
         return element
     
     def hyd_rdom_attach_to_root(self, html : str) -> None:
         """
-            atttach page to root
-            args:
-                page: Page
+        DOM operation: attaches compiled_comp to mounted_comp_id
+
+        Args:
+            html: str - the HTML string to be attached to the root element
         """
         document.getElementById("root").innerHTML = html
 
     def hyd_rdom_attach_to_mounted_comp(
             self,
             mounted_comp_id: str,
             html: str
     ):
         """
-            DOM operation : attaches compiled_comp to mounted_comp_id
-            args:
-                mounted_comp_id: str previosuly mounted component id
-                compiled_comp: str compiled html from comp.render()
+        DOM operation: attaches compiled_comp to mounted_comp_id
+
+        Args:
+            mounted_comp_id: str - the ID of the previously mounted component
+            html: str - the HTML string to be attached to the mounted component
         """
         foundNode = document.querySelector(f'[{ZENAURA_DOM_ATTRIBUTE}="{mounted_comp_id}"]')
         if foundNode:
             foundNode.outerHTML = html
 
     def hyd_rdom_set_attribute(self, mounted_comp_id: str, attribute: Attribute) -> None:
         """
@@ -80,33 +88,46 @@
         element = document.querySelector(f'[{ZENAURA_DOM_ATTRIBUTE}="{mounted_comp_id}"]')
         if element:
             element.removeAttribute(attribute_name)
 
     def hyd_rdom_remove_element(self, mounted_comp_id: str) -> None:
         """
         DOM operation: removes an element from the DOM
-        args:
-            mounted_comp_id: str
+
+        Args:
+            mounted_comp_id: str - the ID of the element to be removed
         """
         element = document.querySelector(f'[{ZENAURA_DOM_ATTRIBUTE}="{mounted_comp_id}"]')
         if element:
             element.parentNode.removeChild(element)
    
     
     def hyd_rdom_append_child(self, mounted_comp_id:str, child_html:str) -> None:
         """
         DOM operation: appends a child to an element
+
+        Args:
+            mounted_comp_id: str - the ID of the parent element
+            child_html: str - the HTML string of the child element to be appended
         """
         element = document.querySelector(f'[{ZENAURA_DOM_ATTRIBUTE}="{mounted_comp_id}"]')
         if element:
             child_node = document.createElement("template")
             child_node.innerHTML = child_html
             element.appendChild(child_node.content.firstChild)
 
     def hyd_rdom_append_child_after(self, parent_node_id, child_node_id, child_html) -> None:
+        """
+        DOM operation: appends a child to an element after a specific child
+
+        Args:
+            parent_node_id: str - the ID of the parent element
+            child_node_id: str - the ID of the child element to insert after
+            child_html: str - the HTML string of the child element to be appended
+        """
         element = document.querySelector(f'[{ZENAURA_DOM_ATTRIBUTE}="{parent_node_id}"]')
         if element : # if parent exists
             child_node = document.createElement("template")
             child_node.innerHTML = child_html
             curr_node = child_node.content.firstChild
             child_index = int( child_node_id[-1])
             prev_child = child_index - 1 # child on the dom to insert the new child after it
@@ -117,71 +138,104 @@
             else: # parent is a leaf no children
                 element.append(curr_node)
             pass
 
     def hyd_rdom_remove_child(self, child_id:str) -> None:
         """
         DOM operation: removes a child of an element
+
+        Args:
+            child_id: str - the ID of the child element to be removed
         """
         child_node = document.querySelector(f'[{ZENAURA_DOM_ATTRIBUTE}="{child_id}"]')
         if child_node:
             child_node.outerHTML = ""
 
 
     def hyd_rdom_add_text_render(self, mounted_comp_id: str, text_content: str) -> None:
         """
         DOM operation: Adds a text node to an element.
+
+        Args:
+            mounted_comp_id: str - the ID of the element to add the text node to
+            text_content: str - the text content of the text node
         """
         element = document.querySelector(f'[{ZENAURA_DOM_ATTRIBUTE}="{mounted_comp_id}"]')
         if element:
             text_node = document.createTextNode(text_content)
             element.appendChild(text_node)
             
 
     def hyd_rdom_replace_inner_text(self, mounted_comp_id: str, new_text: str) -> None:
         """
         DOM operation: Replaces the inner text content of an element.
+
+        Args:
+            mounted_comp_id: str - the ID of the element to replace the text content of
+            new_text: str - the new text content
         """
         element = document.querySelector(f'[{ZENAURA_DOM_ATTRIBUTE}="{mounted_comp_id}"]')
         if element:
             element.textContent = new_text
 
     def hyd_rdom_is_interactive(self) -> bool:
         """
         DOM operation: checks if real dom  is interactive
+
+        Returns:
+            bool - True if the DOM is interactive, False otherwise
         """
         return document.readyState == "interactive"
 
     def hyd_rdom_is_complete(self) -> bool:
         """
         DOM operation: checks if real dom  is complete
+
+        Returns:
+            bool - True if the DOM is complete, False otherwise
         """
         return document.readyState == "complete"
     
     def hyd_rdom_is_loading(self) -> bool:
         """
-        DOM operation: checks if real dom  is loading
+        DOM operation: checks if real dom  is complete
+
+        Returns:
+            bool - True if the DOM is complete, False otherwise
         """
         return document.readyState == "load"
     
     def hyd_rdom_is_content_loaded(self) -> bool:
         """
         DOM operation: checks if real dom  is content loaded
+
+        Returns:
+            bool - True if the DOM is content loaded, False otherwise
         """
         return document.readyState == "DOMContentLoaded"
 
     async def hyd_rdom_wait_for_dom_content_loaded(self):
+        """
+        Waits for the DOM to be content loaded.
+        """
         if not in_browser:
             return 
         while True:
             await asyncio.sleep(0.001)
             if document.readyState=="complete":
                 break
         
 
     def hyd_rdom_toggle_pages_visibilty(self, previous_page : Page, current_page : Page ):
+        """
+        Toggles the visibility of the previous and current pages.
+
+        Args:
+            previous_page: Page - the previously mounted page
+            current_page: Page - the currently mounted page
+        """
         p_page = document.querySelector(f'[data-zenaura="{previous_page.id}"]')
         if p_page:
             p_page.hidden = True
         curr_page = document.querySelector(f'[data-zenaura="{current_page.id}"]')
         if curr_page:
             curr_page.hidden = False # Update the title
```

### Comparing `zenaura-0.9.96/zenaura/client/hydrator/virtual_dom_adapter.py` & `zenaura-0.9.97/zenaura/client/hydrator/virtual_dom_adapter.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.96/zenaura/client/tags/builder.py` & `zenaura-0.9.97/zenaura/client/tags/builder.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,165 +1,173 @@
 from .attribute import Attribute
 from .node import Node
 
 class Builder:
-    def __init__(self, name : str ="div") -> None:
+    """
+    A builder class for constructing HTML tags.
+
+    This class provides a fluent interface for creating HTML tags with attributes,
+    children, and styles. It simplifies the process of building complex HTML structures.
+
+    Attributes:
+        node (Node): The root node of the tag being built.
+    """
+
+    def __init__(self, name: str = "div") -> None:
         """
-        Initializes a Builder object with the given name.
+        Initializes a Builder object with the given tag name.
 
         Args:
-        name (str): The name of the tag.
+            name (str, optional): The name of the tag. Defaults to "div".
         """
         self.node = Node(name)
-    
+
     def with_attributes(self, **kwargs) -> "Builder":
         """
         Adds attributes to the tag.
 
         Args:
             **kwargs: Key-value pairs of attributes.
 
         Returns:
             Builder: The Builder object.
         """
         for key, value in kwargs.items():
             self.with_attribute(key, value)
         return self
-    
+
     def with_children(self, *children) -> "Builder":
         """
         Adds child nodes to the tag.
 
         Args:
             *children: List of child nodes.
 
         Returns:
             Builder: The Builder object.
         """
         for child in children:
             self.with_child(child)
         return self
-    
-    def with_attribute(self, key : str, value : any) -> "Builder":
+
+    def with_attribute(self, key: str, value: any) -> "Builder":
         """
         Adds an attribute to the tag.
 
         Args:
-        key (str): The key of the attribute.
-        value: The value of the attribute.
+            key (str): The key of the attribute.
+            value: The value of the attribute.
 
         Returns:
-        Builder: The Builder object.
+            Builder: The Builder object.
         """
-        self.node.attributes.append(Attribute(key,value))
+        self.node.attributes.append(Attribute(key, value))
         return self
-    
-    def with_child(self, child : Node) -> "Builder":
+
+    def with_child(self, child: Node) -> "Builder":
         """
         Adds a child node to the tag.
 
         Args:
-        child (Node): The child node to be added.
+            child (Node): The child node to be added.
 
         Returns:
-        Builder: The Builder object.
+            Builder: The Builder object.
         """
         self.node.append_child(child)
-        return self 
-    
+        return self
+
     def with_styles(self, styles: dict) -> "Builder":
         """
         Adds styles to the tag.
 
         Args:
-        styles (dict): Dictionary of styles.
+            styles (dict): Dictionary of styles.
 
         Returns:
-        Builder: The Builder object.
+            Builder: The Builder object.
         """
         style_str = ";".join([f"{k}:{v}" for k, v in styles.items()])
         self.node.attributes.append(Attribute("style", style_str))
         return self
-    
-    def with_classes(self, *class_names: str) -> "Builder":
 
+    def with_classes(self, *class_names: str) -> "Builder":
         """
         Adds multiple class names to the element.
 
         Args:
-        *class_names (str): Variable number of class names.
+            *class_names (str): Variable number of class names.
 
         Returns:
-        Builder: The Builder object.
+            Builder: The Builder object.
         """
         for class_name in class_names:
             self.with_class(class_name)
         return self
-    
+
     def with_class(self, class_name: str) -> "Builder":
         """
         Adds a single class name to the element.
 
         Args:
-        class_name (str): The class name to be added.
+            class_name (str): The class name to be added.
 
         Returns:
-        Builder: The Builder object.
+            Builder: The Builder object.
         """
         for i in self.node.attributes:
-            if i.key =="class":
+            if i.key == "class":
                 if class_name not in i.value:
-                    i.value = i.value + " " +  class_name
+                    i.value = i.value + " " + class_name
                     return self
         self.node.attributes.append(Attribute("class", class_name))
-       
+
         return self
 
     def with_class_if(self, class_name: str, condition: bool) -> "Builder":
         """
         Adds a class name to the element if the condition is True.
         If the condition is False, the class is not added.
 
-        args : 
+        args:
             class_name (str): The class name to be added.
             condition (bool): The condition for adding the class.
         """
         self.with_class(class_name) if condition else None
-        return self 
+        return self
 
-    def with_attribute_if(self, key : str, value : any, condition: bool) -> "Builder":
+    def with_attribute_if(self, key: str, value: any, condition: bool) -> "Builder":
         """
-            adds attribute if condition is true 
-            args :
+            adds attribute if condition is true
+            args:
             key (str): The key of the attribute.
             value: The value of the attribute.
             condition (bool): The condition for adding the attribute.
         """
         self.with_attribute(key, value) if condition else None
         return self
-    
-    def with_child_if(self, child : Node, condition: bool) -> "Builder":
+
+    def with_child_if(self, child: Node, condition: bool) -> "Builder":
         """
             adds child if condition is true
-            args :
+            args:
             child (Node): The child node to be added.
             condition (bool): The condition for adding the child.
         """
         self.with_child(child) if condition else None
         return self
-    
-    def with_text(self, text : str):
+
+    def with_text(self, text: str):
         """
             add text node
         """
         self.with_child(Node(text=text))
         return self
 
-    
-    def build(self):
+    def build(self) -> Node:
         """
         Builds and returns the node.
 
         Returns:
-        Node: The built node.
+            Node: The built node.
         """
-        return self.node
+        return self.node
```

### Comparing `zenaura-0.9.96/zenaura/client/tags/node.py` & `zenaura-0.9.97/zenaura/client/tags/node.py`

 * *Files 25% similar despite different names*

```diff
@@ -41,20 +41,27 @@
     def __init__(
             self,name : str = None, 
             children: Optional[List["Node"]]=None, 
             attributes : Optional[List[Attribute]]=None,
             text: str = None,
             ):
         """
-        Initializes a Node object with the given name, children, and attributes.
+        Represents an HTML element with attributes, children, and text content.
 
-        Args:
-        name (str): The name of the node.
-        children (list, optional): List of children nodes. Defaults to None.
-        attributes (list, optional): List of attributes. Defaults to None.
+        Attributes:
+            name (str): The tag name of the element.
+            children (list of Node): The child elements of this node.
+            attributes (list of Attribute): The attributes of this node.
+            text (str, optional): The text content of this node.
+            nodeId (str): A unique identifier for this node.
+            is_leaf (bool): Whether this node has no children.
+            is_text_node (bool): Whether this node represents text content.
+            level (int): The depth of this node in the tree.
+            key (int): A unique identifier for this node within its level.
+            path (str): The path from the root to this node.
         """
         self._parent = None
 
         # calculated properties
         self._level = 0
         self._key = 0 
         self._is_leaf = True
@@ -125,23 +132,33 @@
     @children.setter
     def children(self, new_children):
         """Intercept assignment to update child relationships"""
         self._children = new_children
         update_root_properties(self)
 
     def append_child(self, child):
+        """
+        Adds a child node to this node.
+
+        Args:
+            child (Node or str): The child node to add. If a string is provided,
+                it will be converted to a text node.
+        """
         if isinstance(child, str):
             child = Node(text=child)
             child.is_text_node = True
         self.children.append(child)
         update_root_properties(self)
     
     def to_dict(self) -> dict:
         """
-            convert a node object into nested dictionary.
+        Converts this node and its children into a nested dictionary representation.
+
+        Returns:
+            dict: A dictionary representing the node and its children.
         """
         return {
             "name": self.name,
             "parent": self.parent.name if self.parent else "none",
             "level" : self.level,
             "key": self.key,
             "path": self.path,
@@ -152,15 +169,18 @@
         attrs = []
         for attr in node.attributes:
             attrs.append(f' {attr.key}="{attr.value}"')
         return "".join(attrs)
     
     def to_html(self) -> str:
         """
-            convert a node object into html string.
+        Converts this node and its children into an HTML string.
+
+        Returns:
+            str: The HTML representation of the node and its children.
         """
         if self.name in self_closing_tags:
             return f"<{self.name}{self.getAttributes(self)}>"
         
         html = f"<{self.name}"
         html += f"{self.getAttributes(self)}"
         html += ">"
@@ -172,154 +192,170 @@
             else:
                 html += str(child)
         html += f"</{self.name}>"
         return html
     
     def findChildByName(self, name : str) -> "Node":
         """
-            find a child node by name.
-            args :
-                name - child name
-            returns :
-                None | Node
+        Finds a child node with the given name.
+
+        Args:
+            name (str): The name of the child node to find.
+
+        Returns:
+            Node: The child node with the given name, or None if not found.
         """
         for child in self.children:
             if isinstance(child, Node):
                 if child.name == name:
                     return child
         return None 
     
     def findAllByName(self, name) -> List["Node"]:
         """
-            find all children by name.
-            args :
-                name - child name
-            returns:
-                List["Node"] | []
+        Finds all child nodes with the given name.
+
+        Args:
+            name (str): The name of the child nodes to find.
+
+        Returns:
+            List[Node]: A list of child nodes with the given name.
         """
         found = []
         for child in self.children:
             if isinstance(child, Node):
                 if child.name == name:
                     found.append(child)
 
         return found 
     
     def findByAttribute(self, key : str, value : str) -> "Node":
         """
-            find a child node by attribute key and value.
-            args :
-                name - child name
-            returns:
-                "Node" | None
+        Finds a child node with the given attribute key and value.
+
+        Args:
+            key (str): The attribute key to search for.
+            value (str): The attribute value to search for.
+
+        Returns:
+            Node: The child node with the given attribute, or None if not found.
         """
         found = None
         for child in self.children:
             if isinstance(child, Node):
                 for attribute in child.attributes:
                     if attribute.key == key and attribute.value == value:
                         return child
         return found 
     
     def findAllChildrenByAttributeKey(self, key : str) -> List["Node"]:
         """
-            find all node children by attribute key.
-            args :
-                name - child name
-            returns:
-                list of nodes or empty list
+        Finds all child nodes with the given attribute key.
+
+        Args:
+            key (str): The attribute key to search for.
+
+        Returns:
+            List[Node]: A list of child nodes with the given attribute key.
         """
         found = []
         for child in self.children:
             if isinstance(child, Node):
                 for attribute in child.attributes:
                     if attribute.key == key :
                         found.append(child)
                         break
         return found 
     
     def findAllChildrenByAttributeValue(self, value : str) -> List["Node"]:
         """
-            find all node children by attribute key.
-            args :
-                name - child name
-            returns:
-                list of nodes or empty list
+        Finds all child nodes with the given attribute value.
+
+        Args:
+            value (str): The attribute value to search for.
+
+        Returns:
+            List[Node]: A list of child nodes with the given attribute value.
         """
         found = []
         for child in self.children:
             if isinstance(child, Node):
                 for attribute in child.attributes:
                     if attribute.value == value :
                         found.append(child)
                         break
         return found
     
     def replace(self, oldNode : "Node", newNode: "Node") -> None:
         """
-            replace node child with a new node
-            args :
-                name - child name
-                newNew - new node to replace child with
-            returns:
-                None
+        Replaces a child node with a new node.
+
+        Args:
+            oldNode (Node): The node to be replaced.
+            newNode (Node): The new node to replace it with.
         """
         found = self.getChildIndex(oldNode)
         if found:
             self.children[found] = newNode
     
     def getChildIndex(self,node : "Node") -> int :
         """
-            get child index 
-            args :
-                name - child name
-            returns:
-                int
+        Gets the index of a child node.
+
+        Args:
+            node (Node): The child node to find the index of.
+
+        Returns:
+            int: The index of the child node, or -1 if not found.
         """
         for idx, child in enumerate(self.children):
               if isinstance(child, Node):
                 if child.nodeId == node.nodeId:
                     return idx
                 
     def insertAfter(self, node : "Node", newNode : "Node") -> None:
         """
-            insert new child node after a specific child
-            args :
-                name - child name
-                newNode - node instance
-            returns:
-                int
+        Inserts a new node after a specific child node.
+
+        Args:
+            node (Node): The child node to insert after.
+            newNode (Node): The new node to insert.
         """
         foundIdx = self.getChildIndex(node)
         if foundIdx:
             self.children.insert(foundIdx + 1, newNode)
     
     def insertBefore(self, node : "Node", newNode : "Node") -> None:
         """
-            insert new child node before a specific child
-            args :
-                name - child name
-            returns:
-                int
+        Inserts a new node before a specific child node.
+
+        Args:
+            node (Node): The child node to insert before.
+            newNode (Node): The new node to insert.
         """
         foundIdx = self.getChildIndex(node)
         if foundIdx:
             self.children.insert(foundIdx, newNode)
 
     def remove(self, node : "Node"):
+        """
+        Removes a child node.
+
+        Args:
+            node (Node): The child node to remove.
+        """
         foundIdx = self.getChildIndex(node)
         if foundIdx:
             del self.children[foundIdx]
 
     def appendAttributeToChild(self, node : "Node", attribute : "Attribute") -> None:
-            """
-                appendAttribute to child
-                args :
-                    name - child name
-                    newNew - new node to replace child with
-                returns:
-                    None
-            """
-            for child in self.children:
-              if isinstance(child, Node):
+        """
+        Appends an attribute to a child node.
+
+        Args:
+            node (Node): The child node to add the attribute to.
+            attribute (Attribute): The attribute to add.
+        """
+        for child in self.children:
+            if isinstance(child, Node):
                 if child.nodeId == node.nodeId:
                     child.attributes.append(attribute)
```

### Comparing `zenaura-0.9.96/zenaura.egg-info/PKG-INFO` & `zenaura-0.9.97/zenaura.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zenaura
-Version: 0.9.96
+Version: 0.9.97
 Summary: Zenaura is an experimental Python library built upon PyScript, designed to empower Python developers to create stateful, component-based Single Page Applications (SPAs). By leveraging a virtual DOM implementation, Zenaura optimizes the performance, reactivity, responsiveness, and interactivity of web applications. This allows developers to build high-performance, dynamic web applications using familiar Python concepts and syntax.
 Author: Ahmed Rakan
 Author-email: ar.aldhafeeri11@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bleach
```

### Comparing `zenaura-0.9.96/zenaura.egg-info/SOURCES.txt` & `zenaura-0.9.97/zenaura.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 zenaura.egg-info/top_level.txt
 zenaura/client/__init__.py
 zenaura/client/app.py
 zenaura/client/component.py
 zenaura/client/config.py
 zenaura/client/mocks.py
 zenaura/client/mutator.py
-zenaura/client/observer.py
 zenaura/client/page.py
 zenaura/client/persistance.py
 zenaura/client/algorithm/__init__.py
 zenaura/client/algorithm/algorithm.py
 zenaura/client/algorithm/operations.py
 zenaura/client/algorithm/searcher.py
 zenaura/client/algorithm/updater.py
@@ -53,12 +52,11 @@
 zenaura/client/hydrator/virtual_dom_adapter.py
 zenaura/client/observer/__init__.py
 zenaura/client/observer/observer.py
 zenaura/client/observer/subject.py
 zenaura/client/tags/__init__.py
 zenaura/client/tags/attribute.py
 zenaura/client/tags/builder.py
-zenaura/client/tags/data.py
 zenaura/client/tags/html.py
 zenaura/client/tags/node.py
 zenaura/server/__init__.py
 zenaura/server/server.py
```

