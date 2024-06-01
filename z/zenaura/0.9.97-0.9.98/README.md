# Comparing `tmp/zenaura-0.9.97.tar.gz` & `tmp/zenaura-0.9.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zenaura-0.9.97.tar", last modified: Sat Jun  1 17:55:36 2024, max compression
+gzip compressed data, was "zenaura-0.9.98.tar", last modified: Sat Jun  1 17:59:31 2024, max compression
```

## Comparing `zenaura-0.9.97.tar` & `zenaura-0.9.98.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 17:55:36.465055 zenaura-0.9.97/
--rw-rw-rw-   0        0        0     1100 2024-05-11 11:29:30.000000 zenaura-0.9.97/LICENSE
--rw-rw-rw-   0        0        0     2028 2024-06-01 17:55:36.464556 zenaura-0.9.97/PKG-INFO
--rw-rw-rw-   0        0        0     1376 2024-05-26 16:54:28.000000 zenaura-0.9.97/README.md
--rw-rw-rw-   0        0        0       42 2024-06-01 17:55:36.465055 zenaura-0.9.97/setup.cfg
--rw-rw-rw-   0        0        0     1135 2024-06-01 17:55:10.000000 zenaura-0.9.97/setup.py
-drwxrwxrwx   0        0        0        0 2024-06-01 17:55:36.423051 zenaura-0.9.97/tests/
--rw-rw-rw-   0        0        0    33440 2024-05-26 17:44:57.000000 zenaura-0.9.97/tests/test_algorithm.py
--rw-rw-rw-   0        0        0     6595 2024-05-27 20:30:05.000000 zenaura-0.9.97/tests/test_app.py
--rw-rw-rw-   0        0        0     7595 2024-05-26 17:44:57.000000 zenaura-0.9.97/tests/test_compiler.py
--rw-rw-rw-   0        0        0     4161 2024-05-26 17:44:57.000000 zenaura-0.9.97/tests/test_component_e2e.py
--rw-rw-rw-   0        0        0     1415 2024-05-26 17:44:57.000000 zenaura-0.9.97/tests/test_component_unit.py
--rw-rw-rw-   0        0        0     5301 2024-05-26 17:44:57.000000 zenaura-0.9.97/tests/test_node_properties.py
--rw-rw-rw-   0        0        0     1435 2024-05-26 17:44:57.000000 zenaura-0.9.97/tests/test_observer.py
--rw-rw-rw-   0        0        0     5710 2024-05-26 17:44:57.000000 zenaura-0.9.97/tests/test_rdom_adapter.py
--rw-rw-rw-   0        0        0     1201 2024-05-27 20:12:21.000000 zenaura-0.9.97/tests/test_server.py
--rw-rw-rw-   0        0        0    15215 2024-05-26 17:44:57.000000 zenaura-0.9.97/tests/test_tags.py
--rw-rw-rw-   0        0        0     3293 2024-05-26 17:44:57.000000 zenaura-0.9.97/tests/test_tasker.py
--rw-rw-rw-   0        0        0     5456 2024-05-26 17:44:57.000000 zenaura-0.9.97/tests/test_zenaura_dom.py
-drwxrwxrwx   0        0        0        0 2024-06-01 17:55:36.423550 zenaura-0.9.97/zenaura/
--rw-rw-rw-   0        0        0        0 2024-05-26 19:08:09.000000 zenaura-0.9.97/zenaura/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-01 17:55:36.436052 zenaura-0.9.97/zenaura/client/
--rw-rw-rw-   0        0        0        0 2024-05-26 18:57:31.000000 zenaura-0.9.97/zenaura/client/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-01 17:55:36.439052 zenaura-0.9.97/zenaura/client/algorithm/
--rw-rw-rw-   0        0        0       39 2024-05-26 17:44:57.000000 zenaura-0.9.97/zenaura/client/algorithm/__init__.py
--rw-rw-rw-   0        0        0     1516 2024-05-30 17:33:35.000000 zenaura-0.9.97/zenaura/client/algorithm/algorithm.py
--rw-rw-rw-   0        0        0      972 2024-05-26 17:44:57.000000 zenaura-0.9.97/zenaura/client/algorithm/operations.py
--rw-rw-rw-   0        0        0     9510 2024-05-30 18:06:30.000000 zenaura-0.9.97/zenaura/client/algorithm/searcher.py
--rw-rw-rw-   0        0        0     4602 2024-05-30 17:50:50.000000 zenaura-0.9.97/zenaura/client/algorithm/updater.py
--rw-rw-rw-   0        0        0    11549 2024-05-30 18:20:25.000000 zenaura-0.9.97/zenaura/client/app.py
-drwxrwxrwx   0        0        0        0 2024-06-01 17:55:36.440552 zenaura-0.9.97/zenaura/client/compiler/
--rw-rw-rw-   0        0        0       53 2024-05-26 17:44:57.000000 zenaura-0.9.97/zenaura/client/compiler/__init__.py
--rw-rw-rw-   0        0        0     1995 2024-05-30 17:53:18.000000 zenaura-0.9.97/zenaura/client/compiler/attribute.py
--rw-rw-rw-   0        0        0     4304 2024-05-30 18:06:35.000000 zenaura-0.9.97/zenaura/client/compiler/compiler.py
--rw-rw-rw-   0        0        0     1821 2024-05-30 17:55:09.000000 zenaura-0.9.97/zenaura/client/compiler/sanitize.py
--rw-rw-rw-   0        0        0     6018 2024-05-30 18:21:42.000000 zenaura-0.9.97/zenaura/client/component.py
--rw-rw-rw-   0        0        0      744 2024-05-26 17:44:57.000000 zenaura-0.9.97/zenaura/client/config.py
-drwxrwxrwx   0        0        0        0 2024-06-01 17:55:36.443050 zenaura-0.9.97/zenaura/client/dom/
--rw-rw-rw-   0        0        0       43 2024-05-26 17:44:57.000000 zenaura-0.9.97/zenaura/client/dom/__init__.py
--rw-rw-rw-   0        0        0     1243 2024-05-30 17:57:32.000000 zenaura-0.9.97/zenaura/client/dom/dom.py
--rw-rw-rw-   0        0        0     2969 2024-05-30 17:58:34.000000 zenaura-0.9.97/zenaura/client/dom/error.py
-drwxrwxrwx   0        0        0        0 2024-06-01 17:55:36.444551 zenaura-0.9.97/zenaura/client/dom/lifecycles/
--rw-rw-rw-   0        0        0      930 2024-05-30 17:56:03.000000 zenaura-0.9.97/zenaura/client/dom/lifecycles/mount.py
--rw-rw-rw-   0        0        0     1557 2024-05-30 17:56:46.000000 zenaura-0.9.97/zenaura/client/dom/lifecycles/render.py
--rw-rw-rw-   0        0        0     2700 2024-05-30 17:59:41.000000 zenaura-0.9.97/zenaura/client/dom/mount.py
--rw-rw-rw-   0        0        0     4547 2024-05-30 18:01:23.000000 zenaura-0.9.97/zenaura/client/dom/render.py
-drwxrwxrwx   0        0        0        0 2024-06-01 17:55:36.448051 zenaura-0.9.97/zenaura/client/hydrator/
--rw-rw-rw-   0        0        0      235 2024-05-26 17:44:57.000000 zenaura-0.9.97/zenaura/client/hydrator/__init__.py
--rw-rw-rw-   0        0        0     2041 2024-05-30 17:37:43.000000 zenaura-0.9.97/zenaura/client/hydrator/compiler_adapter.py
--rw-rw-rw-   0        0        0     1193 2024-05-30 17:38:53.000000 zenaura-0.9.97/zenaura/client/hydrator/hydrator.py
--rw-rw-rw-   0        0        0     1376 2024-05-30 17:39:44.000000 zenaura-0.9.97/zenaura/client/hydrator/lookup.py
--rw-rw-rw-   0        0        0     8918 2024-05-30 17:45:58.000000 zenaura-0.9.97/zenaura/client/hydrator/real_dom_adapter.py
--rw-rw-rw-   0        0        0     3441 2024-05-30 17:47:33.000000 zenaura-0.9.97/zenaura/client/hydrator/tasker.py
--rw-rw-rw-   0        0        0     1064 2024-05-26 18:57:08.000000 zenaura-0.9.97/zenaura/client/hydrator/virtual_dom_adapter.py
--rw-rw-rw-   0        0        0     7226 2024-05-30 18:23:13.000000 zenaura-0.9.97/zenaura/client/mocks.py
--rw-rw-rw-   0        0        0     1223 2024-05-30 18:24:01.000000 zenaura-0.9.97/zenaura/client/mutator.py
-drwxrwxrwx   0        0        0        0 2024-06-01 17:55:36.449550 zenaura-0.9.97/zenaura/client/observer/
--rw-rw-rw-   0        0        0       60 2024-05-26 17:44:57.000000 zenaura-0.9.97/zenaura/client/observer/__init__.py
--rw-rw-rw-   0        0        0     2674 2024-05-30 18:02:13.000000 zenaura-0.9.97/zenaura/client/observer/observer.py
--rw-rw-rw-   0        0        0     3384 2024-05-30 18:03:02.000000 zenaura-0.9.97/zenaura/client/observer/subject.py
--rw-rw-rw-   0        0        0     1346 2024-05-30 18:25:55.000000 zenaura-0.9.97/zenaura/client/page.py
--rw-rw-rw-   0        0        0     4235 2024-05-30 18:26:50.000000 zenaura-0.9.97/zenaura/client/persistance.py
-drwxrwxrwx   0        0        0        0 2024-06-01 17:55:36.452551 zenaura-0.9.97/zenaura/client/tags/
--rw-rw-rw-   0        0        0      141 2024-05-30 18:06:40.000000 zenaura-0.9.97/zenaura/client/tags/__init__.py
--rw-rw-rw-   0        0        0      925 2024-05-30 18:04:18.000000 zenaura-0.9.97/zenaura/client/tags/attribute.py
--rw-rw-rw-   0        0        0     5021 2024-05-30 18:05:15.000000 zenaura-0.9.97/zenaura/client/tags/builder.py
--rw-rw-rw-   0        0        0     1325 2024-05-30 18:08:24.000000 zenaura-0.9.97/zenaura/client/tags/html.py
--rw-rw-rw-   0        0        0    11710 2024-05-30 18:13:18.000000 zenaura-0.9.97/zenaura/client/tags/node.py
-drwxrwxrwx   0        0        0        0 2024-06-01 17:55:36.463055 zenaura-0.9.97/zenaura/server/
--rw-rw-rw-   0        0        0       33 2024-05-26 19:08:17.000000 zenaura-0.9.97/zenaura/server/__init__.py
--rw-rw-rw-   0        0        0    12254 2024-06-01 17:54:54.000000 zenaura-0.9.97/zenaura/server/server.py
-drwxrwxrwx   0        0        0        0 2024-06-01 17:55:36.464055 zenaura-0.9.97/zenaura.egg-info/
--rw-rw-rw-   0        0        0     2028 2024-06-01 17:55:36.000000 zenaura-0.9.97/zenaura.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1833 2024-06-01 17:55:36.000000 zenaura-0.9.97/zenaura.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 17:55:36.000000 zenaura-0.9.97/zenaura.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-06-01 17:55:36.000000 zenaura-0.9.97/zenaura.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-06-01 17:55:36.000000 zenaura-0.9.97/zenaura.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 17:59:31.499854 zenaura-0.9.98/
+-rw-rw-rw-   0        0        0     1100 2024-05-11 11:29:30.000000 zenaura-0.9.98/LICENSE
+-rw-rw-rw-   0        0        0     2028 2024-06-01 17:59:31.499353 zenaura-0.9.98/PKG-INFO
+-rw-rw-rw-   0        0        0     1376 2024-05-26 16:54:28.000000 zenaura-0.9.98/README.md
+-rw-rw-rw-   0        0        0       42 2024-06-01 17:59:31.499854 zenaura-0.9.98/setup.cfg
+-rw-rw-rw-   0        0        0     1135 2024-06-01 17:59:12.000000 zenaura-0.9.98/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 17:59:31.457853 zenaura-0.9.98/tests/
+-rw-rw-rw-   0        0        0    33440 2024-05-26 17:44:57.000000 zenaura-0.9.98/tests/test_algorithm.py
+-rw-rw-rw-   0        0        0     6595 2024-05-27 20:30:05.000000 zenaura-0.9.98/tests/test_app.py
+-rw-rw-rw-   0        0        0     7595 2024-05-26 17:44:57.000000 zenaura-0.9.98/tests/test_compiler.py
+-rw-rw-rw-   0        0        0     4161 2024-05-26 17:44:57.000000 zenaura-0.9.98/tests/test_component_e2e.py
+-rw-rw-rw-   0        0        0     1415 2024-05-26 17:44:57.000000 zenaura-0.9.98/tests/test_component_unit.py
+-rw-rw-rw-   0        0        0     5301 2024-05-26 17:44:57.000000 zenaura-0.9.98/tests/test_node_properties.py
+-rw-rw-rw-   0        0        0     1435 2024-05-26 17:44:57.000000 zenaura-0.9.98/tests/test_observer.py
+-rw-rw-rw-   0        0        0     5710 2024-05-26 17:44:57.000000 zenaura-0.9.98/tests/test_rdom_adapter.py
+-rw-rw-rw-   0        0        0     1201 2024-05-27 20:12:21.000000 zenaura-0.9.98/tests/test_server.py
+-rw-rw-rw-   0        0        0    15215 2024-05-26 17:44:57.000000 zenaura-0.9.98/tests/test_tags.py
+-rw-rw-rw-   0        0        0     3293 2024-05-26 17:44:57.000000 zenaura-0.9.98/tests/test_tasker.py
+-rw-rw-rw-   0        0        0     5456 2024-05-26 17:44:57.000000 zenaura-0.9.98/tests/test_zenaura_dom.py
+drwxrwxrwx   0        0        0        0 2024-06-01 17:59:31.458351 zenaura-0.9.98/zenaura/
+-rw-rw-rw-   0        0        0        0 2024-05-26 19:08:09.000000 zenaura-0.9.98/zenaura/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 17:59:31.470853 zenaura-0.9.98/zenaura/client/
+-rw-rw-rw-   0        0        0        0 2024-05-26 18:57:31.000000 zenaura-0.9.98/zenaura/client/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 17:59:31.473853 zenaura-0.9.98/zenaura/client/algorithm/
+-rw-rw-rw-   0        0        0       39 2024-05-26 17:44:57.000000 zenaura-0.9.98/zenaura/client/algorithm/__init__.py
+-rw-rw-rw-   0        0        0     1516 2024-05-30 17:33:35.000000 zenaura-0.9.98/zenaura/client/algorithm/algorithm.py
+-rw-rw-rw-   0        0        0      972 2024-05-26 17:44:57.000000 zenaura-0.9.98/zenaura/client/algorithm/operations.py
+-rw-rw-rw-   0        0        0     9510 2024-05-30 18:06:30.000000 zenaura-0.9.98/zenaura/client/algorithm/searcher.py
+-rw-rw-rw-   0        0        0     4602 2024-05-30 17:50:50.000000 zenaura-0.9.98/zenaura/client/algorithm/updater.py
+-rw-rw-rw-   0        0        0    11549 2024-05-30 18:20:25.000000 zenaura-0.9.98/zenaura/client/app.py
+drwxrwxrwx   0        0        0        0 2024-06-01 17:59:31.475852 zenaura-0.9.98/zenaura/client/compiler/
+-rw-rw-rw-   0        0        0       53 2024-05-26 17:44:57.000000 zenaura-0.9.98/zenaura/client/compiler/__init__.py
+-rw-rw-rw-   0        0        0     1995 2024-05-30 17:53:18.000000 zenaura-0.9.98/zenaura/client/compiler/attribute.py
+-rw-rw-rw-   0        0        0     4304 2024-05-30 18:06:35.000000 zenaura-0.9.98/zenaura/client/compiler/compiler.py
+-rw-rw-rw-   0        0        0     1821 2024-05-30 17:55:09.000000 zenaura-0.9.98/zenaura/client/compiler/sanitize.py
+-rw-rw-rw-   0        0        0     6018 2024-05-30 18:21:42.000000 zenaura-0.9.98/zenaura/client/component.py
+-rw-rw-rw-   0        0        0      744 2024-05-26 17:44:57.000000 zenaura-0.9.98/zenaura/client/config.py
+drwxrwxrwx   0        0        0        0 2024-06-01 17:59:31.478353 zenaura-0.9.98/zenaura/client/dom/
+-rw-rw-rw-   0        0        0       43 2024-05-26 17:44:57.000000 zenaura-0.9.98/zenaura/client/dom/__init__.py
+-rw-rw-rw-   0        0        0     1243 2024-05-30 17:57:32.000000 zenaura-0.9.98/zenaura/client/dom/dom.py
+-rw-rw-rw-   0        0        0     2969 2024-05-30 17:58:34.000000 zenaura-0.9.98/zenaura/client/dom/error.py
+drwxrwxrwx   0        0        0        0 2024-06-01 17:59:31.479354 zenaura-0.9.98/zenaura/client/dom/lifecycles/
+-rw-rw-rw-   0        0        0      930 2024-05-30 17:56:03.000000 zenaura-0.9.98/zenaura/client/dom/lifecycles/mount.py
+-rw-rw-rw-   0        0        0     1557 2024-05-30 17:56:46.000000 zenaura-0.9.98/zenaura/client/dom/lifecycles/render.py
+-rw-rw-rw-   0        0        0     2700 2024-05-30 17:59:41.000000 zenaura-0.9.98/zenaura/client/dom/mount.py
+-rw-rw-rw-   0        0        0     4547 2024-05-30 18:01:23.000000 zenaura-0.9.98/zenaura/client/dom/render.py
+drwxrwxrwx   0        0        0        0 2024-06-01 17:59:31.482852 zenaura-0.9.98/zenaura/client/hydrator/
+-rw-rw-rw-   0        0        0      235 2024-05-26 17:44:57.000000 zenaura-0.9.98/zenaura/client/hydrator/__init__.py
+-rw-rw-rw-   0        0        0     2041 2024-05-30 17:37:43.000000 zenaura-0.9.98/zenaura/client/hydrator/compiler_adapter.py
+-rw-rw-rw-   0        0        0     1193 2024-05-30 17:38:53.000000 zenaura-0.9.98/zenaura/client/hydrator/hydrator.py
+-rw-rw-rw-   0        0        0     1376 2024-05-30 17:39:44.000000 zenaura-0.9.98/zenaura/client/hydrator/lookup.py
+-rw-rw-rw-   0        0        0     8918 2024-05-30 17:45:58.000000 zenaura-0.9.98/zenaura/client/hydrator/real_dom_adapter.py
+-rw-rw-rw-   0        0        0     3441 2024-05-30 17:47:33.000000 zenaura-0.9.98/zenaura/client/hydrator/tasker.py
+-rw-rw-rw-   0        0        0     1064 2024-05-26 18:57:08.000000 zenaura-0.9.98/zenaura/client/hydrator/virtual_dom_adapter.py
+-rw-rw-rw-   0        0        0     7226 2024-05-30 18:23:13.000000 zenaura-0.9.98/zenaura/client/mocks.py
+-rw-rw-rw-   0        0        0     1223 2024-05-30 18:24:01.000000 zenaura-0.9.98/zenaura/client/mutator.py
+drwxrwxrwx   0        0        0        0 2024-06-01 17:59:31.484351 zenaura-0.9.98/zenaura/client/observer/
+-rw-rw-rw-   0        0        0       60 2024-05-26 17:44:57.000000 zenaura-0.9.98/zenaura/client/observer/__init__.py
+-rw-rw-rw-   0        0        0     2674 2024-05-30 18:02:13.000000 zenaura-0.9.98/zenaura/client/observer/observer.py
+-rw-rw-rw-   0        0        0     3384 2024-05-30 18:03:02.000000 zenaura-0.9.98/zenaura/client/observer/subject.py
+-rw-rw-rw-   0        0        0     1346 2024-05-30 18:25:55.000000 zenaura-0.9.98/zenaura/client/page.py
+-rw-rw-rw-   0        0        0     4235 2024-05-30 18:26:50.000000 zenaura-0.9.98/zenaura/client/persistance.py
+drwxrwxrwx   0        0        0        0 2024-06-01 17:59:31.486853 zenaura-0.9.98/zenaura/client/tags/
+-rw-rw-rw-   0        0        0      141 2024-05-30 18:06:40.000000 zenaura-0.9.98/zenaura/client/tags/__init__.py
+-rw-rw-rw-   0        0        0      925 2024-05-30 18:04:18.000000 zenaura-0.9.98/zenaura/client/tags/attribute.py
+-rw-rw-rw-   0        0        0     5021 2024-05-30 18:05:15.000000 zenaura-0.9.98/zenaura/client/tags/builder.py
+-rw-rw-rw-   0        0        0     1325 2024-05-30 18:08:24.000000 zenaura-0.9.98/zenaura/client/tags/html.py
+-rw-rw-rw-   0        0        0    11710 2024-05-30 18:13:18.000000 zenaura-0.9.98/zenaura/client/tags/node.py
+drwxrwxrwx   0        0        0        0 2024-06-01 17:59:31.497853 zenaura-0.9.98/zenaura/server/
+-rw-rw-rw-   0        0        0       44 2024-06-01 17:59:04.000000 zenaura-0.9.98/zenaura/server/__init__.py
+-rw-rw-rw-   0        0        0    12250 2024-06-01 17:58:50.000000 zenaura-0.9.98/zenaura/server/server.py
+drwxrwxrwx   0        0        0        0 2024-06-01 17:59:31.498852 zenaura-0.9.98/zenaura.egg-info/
+-rw-rw-rw-   0        0        0     2028 2024-06-01 17:59:31.000000 zenaura-0.9.98/zenaura.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1833 2024-06-01 17:59:31.000000 zenaura-0.9.98/zenaura.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 17:59:31.000000 zenaura-0.9.98/zenaura.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-06-01 17:59:31.000000 zenaura-0.9.98/zenaura.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-06-01 17:59:31.000000 zenaura-0.9.98/zenaura.egg-info/top_level.txt
```

### Comparing `zenaura-0.9.97/LICENSE` & `zenaura-0.9.98/LICENSE`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.97/PKG-INFO` & `zenaura-0.9.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zenaura
-Version: 0.9.97
+Version: 0.9.98
 Summary: Zenaura is an experimental Python library built upon PyScript, designed to empower Python developers to create stateful, component-based Single Page Applications (SPAs). By leveraging a virtual DOM implementation, Zenaura optimizes the performance, reactivity, responsiveness, and interactivity of web applications. This allows developers to build high-performance, dynamic web applications using familiar Python concepts and syntax.
 Author: Ahmed Rakan
 Author-email: ar.aldhafeeri11@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bleach
```

### Comparing `zenaura-0.9.97/README.md` & `zenaura-0.9.98/README.md`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.97/setup.py` & `zenaura-0.9.98/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='zenaura',
-    version='0.9.97',
+    version='0.9.98',
     description="Zenaura is an experimental Python library built upon PyScript, designed to empower Python developers to create stateful, component-based Single Page Applications (SPAs). By leveraging a virtual DOM implementation, Zenaura optimizes the performance, reactivity, responsiveness, and interactivity of web applications. This allows developers to build high-performance, dynamic web applications using familiar Python concepts and syntax.",
     author="Ahmed Rakan",
     author_email="ar.aldhafeeri11@gmail.com",
     packages=['zenaura', 'zenaura.server', 'zenaura.client', 'zenaura.client.algorithm', 'zenaura.client.compiler', 'zenaura.client.hydrator', 'zenaura.client.observer', 'zenaura.client.tags', 'zenaura.client.dom', 'zenaura.client.dom.lifecycles'],
     install_requires=[
         'bleach'
     ],
```

### Comparing `zenaura-0.9.97/tests/test_algorithm.py` & `zenaura-0.9.98/tests/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.97/tests/test_app.py` & `zenaura-0.9.98/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.97/tests/test_compiler.py` & `zenaura-0.9.98/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.97/tests/test_component_e2e.py` & `zenaura-0.9.98/tests/test_component_e2e.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.97/tests/test_component_unit.py` & `zenaura-0.9.98/tests/test_component_unit.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.97/tests/test_node_properties.py` & `zenaura-0.9.98/tests/test_node_properties.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.97/tests/test_observer.py` & `zenaura-0.9.98/tests/test_observer.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.97/tests/test_rdom_adapter.py` & `zenaura-0.9.98/tests/test_rdom_adapter.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.97/tests/test_server.py` & `zenaura-0.9.98/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.97/tests/test_tags.py` & `zenaura-0.9.98/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.97/tests/test_tasker.py` & `zenaura-0.9.98/tests/test_tasker.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.97/tests/test_zenaura_dom.py` & `zenaura-0.9.98/tests/test_zenaura_dom.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.97/zenaura/client/algorithm/algorithm.py` & `zenaura-0.9.98/zenaura/client/algorithm/algorithm.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.97/zenaura/client/algorithm/operations.py` & `zenaura-0.9.98/zenaura/client/algorithm/operations.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.97/zenaura/client/algorithm/searcher.py` & `zenaura-0.9.98/zenaura/client/algorithm/searcher.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.97/zenaura/client/algorithm/updater.py` & `zenaura-0.9.98/zenaura/client/algorithm/updater.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.97/zenaura/client/app.py` & `zenaura-0.9.98/zenaura/client/app.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.97/zenaura/client/compiler/attribute.py` & `zenaura-0.9.98/zenaura/client/compiler/attribute.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.97/zenaura/client/compiler/compiler.py` & `zenaura-0.9.98/zenaura/client/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.97/zenaura/client/compiler/sanitize.py` & `zenaura-0.9.98/zenaura/client/compiler/sanitize.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.97/zenaura/client/component.py` & `zenaura-0.9.98/zenaura/client/component.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.97/zenaura/client/config.py` & `zenaura-0.9.98/zenaura/client/config.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.97/zenaura/client/dom/dom.py` & `zenaura-0.9.98/zenaura/client/dom/dom.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.97/zenaura/client/dom/error.py` & `zenaura-0.9.98/zenaura/client/dom/error.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.97/zenaura/client/dom/lifecycles/mount.py` & `zenaura-0.9.98/zenaura/client/dom/lifecycles/mount.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.97/zenaura/client/dom/lifecycles/render.py` & `zenaura-0.9.98/zenaura/client/dom/lifecycles/render.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.97/zenaura/client/dom/mount.py` & `zenaura-0.9.98/zenaura/client/dom/mount.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.97/zenaura/client/dom/render.py` & `zenaura-0.9.98/zenaura/client/dom/render.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.97/zenaura/client/hydrator/compiler_adapter.py` & `zenaura-0.9.98/zenaura/client/hydrator/compiler_adapter.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.97/zenaura/client/hydrator/hydrator.py` & `zenaura-0.9.98/zenaura/client/hydrator/hydrator.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.97/zenaura/client/hydrator/lookup.py` & `zenaura-0.9.98/zenaura/client/hydrator/lookup.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.97/zenaura/client/hydrator/real_dom_adapter.py` & `zenaura-0.9.98/zenaura/client/hydrator/real_dom_adapter.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.97/zenaura/client/hydrator/tasker.py` & `zenaura-0.9.98/zenaura/client/hydrator/tasker.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.97/zenaura/client/hydrator/virtual_dom_adapter.py` & `zenaura-0.9.98/zenaura/client/hydrator/virtual_dom_adapter.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.97/zenaura/client/mocks.py` & `zenaura-0.9.98/zenaura/client/mocks.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.97/zenaura/client/mutator.py` & `zenaura-0.9.98/zenaura/client/mutator.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.97/zenaura/client/observer/observer.py` & `zenaura-0.9.98/zenaura/client/observer/observer.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.97/zenaura/client/observer/subject.py` & `zenaura-0.9.98/zenaura/client/observer/subject.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.97/zenaura/client/page.py` & `zenaura-0.9.98/zenaura/client/page.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.97/zenaura/client/persistance.py` & `zenaura-0.9.98/zenaura/client/persistance.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.97/zenaura/client/tags/attribute.py` & `zenaura-0.9.98/zenaura/client/tags/attribute.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.97/zenaura/client/tags/builder.py` & `zenaura-0.9.98/zenaura/client/tags/builder.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.97/zenaura/client/tags/html.py` & `zenaura-0.9.98/zenaura/client/tags/html.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.97/zenaura/client/tags/node.py` & `zenaura-0.9.98/zenaura/client/tags/node.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.97/zenaura/server/server.py` & `zenaura-0.9.98/zenaura/server/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -266,17 +266,17 @@
                 Args:
                     event (FileSystemEvent): The file system event.
                 """
 
                 try:
                     logging.info(f"File {event.src_path} has changed.")
                     logging.info("Changes are live...")
-                    self.server.hydrate_and_notify()
+                    DEVSERVER.hydrate_and_notify()
                     logging.info("Reloading browser...")
-                    self.server.send_refresh_signal()
+                    DEVSERVER.send_refresh_signal()
                     logging.info("Browser reloaded.")
                 except Exception as e:
                     logging.info(f"Error in ChangeHandler: {e}")
 
         return ChangeHandler
 
     def start_server(self):
```

#### html2text {}

```diff
@@ -96,28 +96,28 @@
 (FileSystemEventHandler): """ A class that handles file system events. This
 class is used to detect changes in the application files and trigger a refresh
 of the browser. """ def __init__(self, server): """ Initializes the
 ChangeHandler class. Args: server (DevServer): The DevServer instance. """
 super().__init__() self.server = server def on_any_event(self, event): """
 Handles file system events. Args: event (FileSystemEvent): The file system
 event. """ try: logging.info(f"File {event.src_path} has changed.")
-logging.info("Changes are live...") self.server.hydrate_and_notify()
-logging.info("Reloading browser...") self.server.send_refresh_signal()
-logging.info("Browser reloaded.") except Exception as e: logging.info(f"Error
-in ChangeHandler: {e}") return ChangeHandler def start_server(self): """ Starts
-the Flask server. """ try: self.app.run(debug=self.debug, port=self.port,
-use_reloader=False) except Exception as e: logging.info(f"Error starting
-server: {e}") def hydrate_and_notify(self): """ Hydrates the application and
-notifies clients of changes. """ try: self.observer.pause() logging.info
-("Hydrating...") logging.info("Pausing the observer...") process =
-subprocess.Popen("python build.py", shell=True) process.communicate()
-logging.info("Hydrated done...") finally: logging.info("Running the
-observer...") self.observer.resume() def run(self): """ Runs the development
-server. This method starts the Flask server, file system observer, and
-WebSocket server. """ path = 'public' ChangeHandler = self.get_change_handler()
-event_handler = ChangeHandler(self) self.observer.schedule(event_handler, path,
-recursive=True) self.observer.start() server_thread = Thread
-(target=self.start_server, daemon=True) server_thread.start() try: while not
-self.shutdown_event.is_set(): time.sleep(0.1) # Shorter sleep interval except
-KeyboardInterrupt: logging.info("KeyboardInterrupt received, stopping...")
-finally: # Faster Shutdown of Observer self.observer.event_queue.queue.clear()
-self.observer.stop() self.observer.join()
+logging.info("Changes are live...") DEVSERVER.hydrate_and_notify() logging.info
+("Reloading browser...") DEVSERVER.send_refresh_signal() logging.info("Browser
+reloaded.") except Exception as e: logging.info(f"Error in ChangeHandler: {e}")
+return ChangeHandler def start_server(self): """ Starts the Flask server. """
+try: self.app.run(debug=self.debug, port=self.port, use_reloader=False) except
+Exception as e: logging.info(f"Error starting server: {e}") def
+hydrate_and_notify(self): """ Hydrates the application and notifies clients of
+changes. """ try: self.observer.pause() logging.info("Hydrating...")
+logging.info("Pausing the observer...") process = subprocess.Popen("python
+build.py", shell=True) process.communicate() logging.info("Hydrated done...")
+finally: logging.info("Running the observer...") self.observer.resume() def run
+(self): """ Runs the development server. This method starts the Flask server,
+file system observer, and WebSocket server. """ path = 'public' ChangeHandler =
+self.get_change_handler() event_handler = ChangeHandler(self)
+self.observer.schedule(event_handler, path, recursive=True) self.observer.start
+() server_thread = Thread(target=self.start_server, daemon=True)
+server_thread.start() try: while not self.shutdown_event.is_set(): time.sleep
+(0.1) # Shorter sleep interval except KeyboardInterrupt: logging.info
+("KeyboardInterrupt received, stopping...") finally: # Faster Shutdown of
+Observer self.observer.event_queue.queue.clear() self.observer.stop()
+self.observer.join()
```

### Comparing `zenaura-0.9.97/zenaura.egg-info/PKG-INFO` & `zenaura-0.9.98/zenaura.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zenaura
-Version: 0.9.97
+Version: 0.9.98
 Summary: Zenaura is an experimental Python library built upon PyScript, designed to empower Python developers to create stateful, component-based Single Page Applications (SPAs). By leveraging a virtual DOM implementation, Zenaura optimizes the performance, reactivity, responsiveness, and interactivity of web applications. This allows developers to build high-performance, dynamic web applications using familiar Python concepts and syntax.
 Author: Ahmed Rakan
 Author-email: ar.aldhafeeri11@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bleach
```

### Comparing `zenaura-0.9.97/zenaura.egg-info/SOURCES.txt` & `zenaura-0.9.98/zenaura.egg-info/SOURCES.txt`

 * *Files identical despite different names*

