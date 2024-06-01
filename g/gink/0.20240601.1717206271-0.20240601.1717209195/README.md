# Comparing `tmp/gink-0.20240601.1717206271.tar.gz` & `tmp/gink-0.20240601.1717209195.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gink-0.20240601.1717206271.tar", last modified: Sat Jun  1 01:44:34 2024, max compression
+gzip compressed data, was "gink-0.20240601.1717209195.tar", last modified: Sat Jun  1 02:33:18 2024, max compression
```

## Comparing `gink-0.20240601.1717206271.tar` & `gink-0.20240601.1717209195.tar`

### file list

```diff
@@ -1,102 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:44:34.707765 gink-0.20240601.1717206271/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11216 2024-06-01 01:44:34.707765 gink-0.20240601.1717206271/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9857 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:44:34.691765 gink-0.20240601.1717206271/gink/
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7062 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:44:34.695765 gink-0.20240601.1717206271/gink/builders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 01:44:31.000000 gink-0.20240601.1717206271/gink/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-06-01 01:44:31.000000 gink-0.20240601.1717206271/gink/builders/behavior_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-06-01 01:44:31.000000 gink-0.20240601.1717206271/gink/builders/bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-06-01 01:44:31.000000 gink-0.20240601.1717206271/gink/builders/change_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-06-01 01:44:31.000000 gink-0.20240601.1717206271/gink/builders/claim_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-06-01 01:44:31.000000 gink-0.20240601.1717206271/gink/builders/clearance_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-06-01 01:44:31.000000 gink-0.20240601.1717206271/gink/builders/container_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     8918 2024-06-01 01:44:31.000000 gink-0.20240601.1717206271/gink/builders/entry_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-06-01 01:44:31.000000 gink-0.20240601.1717206271/gink/builders/header_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-06-01 01:44:31.000000 gink-0.20240601.1717206271/gink/builders/key_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-06-01 01:44:31.000000 gink-0.20240601.1717206271/gink/builders/log_file_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-06-01 01:44:31.000000 gink-0.20240601.1717206271/gink/builders/movement_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-06-01 01:44:31.000000 gink-0.20240601.1717206271/gink/builders/muid_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-06-01 01:44:31.000000 gink-0.20240601.1717206271/gink/builders/pair_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-06-01 01:44:31.000000 gink-0.20240601.1717206271/gink/builders/sync_message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    40439 2024-06-01 01:44:31.000000 gink-0.20240601.1717206271/gink/builders/value_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:44:34.703765 gink-0.20240601.1717206271/gink/impl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11188 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/abstract_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/addressable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/attribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/box.py
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/braid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/builders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/bundle_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/bundle_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/bundle_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/bundler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/chain_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)    19865 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/coding.py
--rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    13325 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/container.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14405 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/deferred.py
--rw-r--r--   0 runner    (1001) docker     (127)    11594 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/directory.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11218 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/key_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/listener.py
--rw-r--r--   0 runner    (1001) docker     (127)    57325 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/lmdb_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/lmdb_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/log_backed_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/looping.py
--rw-r--r--   0 runner    (1001) docker     (127)    23274 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/memory_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/muid.py
--rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/pair_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/pair_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/property.py
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/selectable_console.py
--rw-r--r--   0 runner    (1001) docker     (127)    12612 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/tuples.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/typedefs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/websocket_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/wsgi_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/wsgi_listener.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:44:34.707765 gink-0.20240601.1717206271/gink/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_braid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_chain_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_change_set_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_code_values.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_demo.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10116 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_key_set.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_lmdb_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_logbackedstore.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_memory_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_muid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_pair_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_pair_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_property.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    10500 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    14345 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_websocket_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_wsgi_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:44:34.707765 gink-0.20240601.1717206271/gink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11216 2024-06-01 01:44:34.000000 gink-0.20240601.1717206271/gink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-06-01 01:44:34.000000 gink-0.20240601.1717206271/gink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 01:44:34.000000 gink-0.20240601.1717206271/gink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-06-01 01:44:34.000000 gink-0.20240601.1717206271/gink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-06-01 01:44:34.000000 gink-0.20240601.1717206271/gink.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 01:44:34.707765 gink-0.20240601.1717206271/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-06-01 01:44:31.000000 gink-0.20240601.1717206271/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:33:18.392736 gink-0.20240601.1717209195/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11216 2024-06-01 02:33:18.392736 gink-0.20240601.1717209195/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9857 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:33:18.376736 gink-0.20240601.1717209195/gink/
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7400 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/braid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:33:18.380736 gink-0.20240601.1717209195/gink/builders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 02:33:15.000000 gink-0.20240601.1717209195/gink/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-06-01 02:33:15.000000 gink-0.20240601.1717209195/gink/builders/behavior_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-06-01 02:33:15.000000 gink-0.20240601.1717209195/gink/builders/bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-06-01 02:33:15.000000 gink-0.20240601.1717209195/gink/builders/change_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-06-01 02:33:15.000000 gink-0.20240601.1717209195/gink/builders/claim_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-06-01 02:33:15.000000 gink-0.20240601.1717209195/gink/builders/clearance_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-06-01 02:33:15.000000 gink-0.20240601.1717209195/gink/builders/container_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8918 2024-06-01 02:33:15.000000 gink-0.20240601.1717209195/gink/builders/entry_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-06-01 02:33:15.000000 gink-0.20240601.1717209195/gink/builders/header_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-06-01 02:33:15.000000 gink-0.20240601.1717209195/gink/builders/key_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-06-01 02:33:15.000000 gink-0.20240601.1717209195/gink/builders/log_file_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-06-01 02:33:15.000000 gink-0.20240601.1717209195/gink/builders/movement_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-06-01 02:33:15.000000 gink-0.20240601.1717209195/gink/builders/muid_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-06-01 02:33:15.000000 gink-0.20240601.1717209195/gink/builders/pair_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-06-01 02:33:15.000000 gink-0.20240601.1717209195/gink/builders/sync_message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40439 2024-06-01 02:33:15.000000 gink-0.20240601.1717209195/gink/builders/value_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:33:18.388736 gink-0.20240601.1717209195/gink/impl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10233 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/impl/abstract_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/impl/addressable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/impl/attribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/impl/box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/impl/braid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/impl/braid_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/impl/builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/impl/bundle_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/impl/bundle_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/impl/bundle_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/impl/bundler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/impl/chain_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19865 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/impl/coding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/impl/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13325 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/impl/container.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9124 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/impl/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/impl/deferred.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11594 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/impl/directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/impl/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/impl/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/impl/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11218 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/impl/key_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/impl/listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57479 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/impl/lmdb_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/impl/lmdb_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/impl/log_backed_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/impl/looping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23274 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/impl/memory_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/impl/muid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/impl/pair_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/impl/pair_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/impl/property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/impl/relay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/impl/selectable_console.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12612 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/impl/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/impl/tuples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/impl/typedefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/impl/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/impl/watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7442 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/impl/websocket_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/impl/wsgi_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/impl/wsgi_listener.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:33:18.392736 gink-0.20240601.1717209195/gink/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/tests/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/tests/test_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/tests/test_braid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/tests/test_chain_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/tests/test_change_set_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/tests/test_code_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/tests/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/tests/test_demo.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10116 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/tests/test_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/tests/test_key_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/tests/test_lmdb_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/tests/test_logbackedstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/tests/test_memory_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/tests/test_muid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/tests/test_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/tests/test_pair_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/tests/test_pair_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/tests/test_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/tests/test_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10500 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/tests/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14345 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/tests/test_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/tests/test_websocket_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-06-01 02:33:13.000000 gink-0.20240601.1717209195/gink/tests/test_wsgi_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:33:18.392736 gink-0.20240601.1717209195/gink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11216 2024-06-01 02:33:18.000000 gink-0.20240601.1717209195/gink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-06-01 02:33:18.000000 gink-0.20240601.1717209195/gink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 02:33:18.000000 gink-0.20240601.1717209195/gink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-06-01 02:33:18.000000 gink-0.20240601.1717209195/gink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-06-01 02:33:18.000000 gink-0.20240601.1717209195/gink.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 02:33:18.392736 gink-0.20240601.1717209195/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-06-01 02:33:15.000000 gink-0.20240601.1717209195/setup.py
```

### Comparing `gink-0.20240601.1717206271/LICENSE` & `gink-0.20240601.1717209195/LICENSE`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/PKG-INFO` & `gink-0.20240601.1717209195/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gink
-Version: 0.20240601.1717206271
+Version: 0.20240601.1717209195
 Summary: a system for storing data structures in lmdb
 Home-page: https://github.com/x5e/gink
 Author: Darin McGill
 Author-email: gink@darinmcgill.com
 Keywords: gink lmdb crdt history versioned
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `gink-0.20240601.1717206271/README.md` & `gink-0.20240601.1717209195/README.md`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/__init__.py` & `gink-0.20240601.1717209195/gink/__init__.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/__main__.py` & `gink-0.20240601.1717209195/gink/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 from logging import basicConfig, getLogger
 from sys import exit, stdin
 from re import fullmatch
 from argparse import ArgumentParser, Namespace
 from pathlib import Path
 from typing import Optional, Tuple, Union
 from importlib import import_module
+from os import environ
 
 from . import *
 from .impl.builders import BundleBuilder
 from .impl.selectable_console import SelectableConsole
-from .impl.utilities import get_identity
+from .impl.utilities import get_identity, make_auth_func
 from .impl.looping import loop
 from .impl.wsgi_listener import WsgiListener
 
 parser: ArgumentParser = ArgumentParser(allow_abbrev=False)
 parser.add_argument("db_path", nargs="?", help="path to a database; created if doesn't exist")
 parser.add_argument("--verbosity", "-v", default="INFO", help="the log level to use, e.g. INFO or DEBUG")
 parser.add_argument("--format", default="lmdb", help="storage file format", choices=["lmdb", "binlog"])
@@ -38,14 +39,15 @@
 parser.add_argument("--line_mode", action="store_true", help="read lines of input from stdin")
 parser.add_argument("--interactive", action="store_true", help="force interactive mode")
 parser.add_argument("--heartbeat_to", type=Path, help="write on console refresh (for debugging)")
 parser.add_argument("--identity", help="explicitly set identity to be associated with changes")
 parser.add_argument("--starts", help="include starting bundles when showing log", action="store_true")
 parser.add_argument("--wsgi", help="serve module.function via wsgi")
 parser.add_argument("--wsgi_listen_on", help="ip:port or port to listen on (defaults to *:8081)")
+parser.add_argument("--auth_token", default=environ.get("GINK_AUTH_TOKEN"), help="auth token for connections")
 args: Namespace = parser.parse_args()
 if args.show_arguments:
     print(args)
     exit(0)
 basicConfig(format="\r[%(asctime)s.%(msecs)03d %(name)s:%(levelname)s] %(message)s",
             level=args.verbosity, datefmt='%I:%M:%S')
 logger = getLogger()
@@ -157,20 +159,23 @@
     imported = import_module(module)
     app = getattr(imported, function, None)
     if not app:
         raise ValueError(f"{function} not found in {module}")
     ip_addr, port = parse_listen_on(args.wsgi_listen_on, "*", "8081")
     wsgi_listener = WsgiListener(app, ip_addr=ip_addr, port=int(port))
 
+auth_func = make_auth_func(args.auth_token) if args.auth_token else None
+
 if args.listen_on:
     ip_addr, port = parse_listen_on(args.listen_on, "*", "8080")
-    database.start_listening(ip_addr=ip_addr, port=port)
+    database.start_listening(ip_addr=ip_addr, port=port, auth_func=auth_func)
 
 for target in (args.connect_to or []):
-    database.connect_to(target)
+    auth_data = f"Token {args.auth_token}" if args.auth_token else None
+    database.connect_to(target, auth_data=auth_data)
 
 if args.interactive:
     interactive = True
 elif args.line_mode:
     interactive = False
 else:
     interactive = stdin.isatty()
```

### Comparing `gink-0.20240601.1717206271/gink/builders/behavior_pb2.py` & `gink-0.20240601.1717209195/gink/builders/behavior_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/builders/bundle_pb2.py` & `gink-0.20240601.1717209195/gink/builders/bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/builders/change_pb2.py` & `gink-0.20240601.1717209195/gink/builders/change_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/builders/claim_pb2.py` & `gink-0.20240601.1717209195/gink/builders/claim_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/builders/clearance_pb2.py` & `gink-0.20240601.1717209195/gink/builders/clearance_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/builders/container_pb2.py` & `gink-0.20240601.1717209195/gink/builders/container_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/builders/entry_pb2.py` & `gink-0.20240601.1717209195/gink/builders/entry_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/builders/header_pb2.py` & `gink-0.20240601.1717209195/gink/builders/header_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/builders/key_pb2.py` & `gink-0.20240601.1717209195/gink/builders/key_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/builders/log_file_pb2.py` & `gink-0.20240601.1717209195/gink/builders/log_file_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/builders/movement_pb2.py` & `gink-0.20240601.1717209195/gink/builders/movement_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/builders/muid_pb2.py` & `gink-0.20240601.1717209195/gink/builders/muid_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/builders/pair_pb2.py` & `gink-0.20240601.1717209195/gink/builders/pair_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/builders/sync_message_pb2.py` & `gink-0.20240601.1717209195/gink/builders/sync_message_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/builders/value_pb2.py` & `gink-0.20240601.1717209195/gink/builders/value_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/impl/abstract_store.py` & `gink-0.20240601.1717209195/gink/impl/abstract_store.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,74 +1,44 @@
 """Contains AbstractStore class."""
 
 # standard python modules
 from typing import Tuple, Optional, Iterable, List, Union, Mapping, TypeVar, Generic, Callable
 from abc import abstractmethod
 
-from pathlib import Path
 
 # Gink specific modules
 from .builders import ContainerBuilder, ChangeBuilder, EntryBuilder, ClaimBuilder
 from .bundle_info import BundleInfo
 from .chain_tracker import ChainTracker
 from .typedefs import UserKey, MuTimestamp, Medallion, Limit
 from .tuples import FoundEntry, Chain, PositionedEntry, FoundContainer
 from .muid import Muid
 from .bundle_wrapper import BundleWrapper
 from .utilities import is_certainly_gone
-from .watcher import Watcher
 from .bundle_store import BundleStore
 Lock = TypeVar('Lock')
 
 
 class AbstractStore(BundleStore, Generic[Lock]):
     """ abstract base class for the gink data store
 
         Stores both the bundles received and the contents of those
         bundles unpacked so that you can examine entries, container definitions, etc.
 
         Warning! Since data stores are viewed as part of the internal implementation,
         this interface may change at any time without warning on a minor version change.
     """
-    on_ready: Callable  # needs to by dynamically assigned
 
     def __enter__(self):
         pass
 
     def __exit__(self, *_):
         self.close()
 
     @abstractmethod
-    def _get_file_path(self) -> Optional[Path]:
-        """ Return the underlying file name, or None if the store isn't file backed.
-        """
-
-    def is_selectable(self) -> bool:
-        return self._get_watcher() is not None
-
-    def _get_watcher(self) -> Optional[Watcher]:
-        if not Watcher.supported():
-            return None
-        file_path = self._get_file_path()
-        if file_path is None:
-            return None
-        if not hasattr(self, "_watcher"):
-            setattr(self, "_watcher", Watcher(file_path))
-        return getattr(self, "_watcher")
-
-    def fileno(self) -> int:
-        watcher = self._get_watcher()
-        assert watcher is not None
-        return watcher.fileno()
-
-    def _clear_notifications(self):
-        if hasattr(self, "_watcher"):
-            self._watcher.clear()
-
-    @abstractmethod
     def get_container(self, container: Muid) -> Optional[ContainerBuilder]:
         """ Gets the container definition associated with a particular address. """
 
     @abstractmethod
     def get_comment(self, *, medallion: Medallion, timestamp: MuTimestamp) -> Optional[str]:
         """ Gets the comment associated with a particular bundle, if stored. """
         raise NotImplementedError()
```

### Comparing `gink-0.20240601.1717206271/gink/impl/addressable.py` & `gink-0.20240601.1717209195/gink/impl/addressable.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/impl/attribution.py` & `gink-0.20240601.1717209195/gink/impl/attribution.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/impl/box.py` & `gink-0.20240601.1717209195/gink/impl/box.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/impl/braid.py` & `gink-0.20240601.1717209195/gink/impl/braid.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" Contains the `Property` Container class. """
+""" Contains the `Braid` Container class, which is primarily intended for internal use in the braid server. """
 from __future__ import annotations
 from typing import Optional, Dict, Tuple, Iterable, Union
 
 from .typedefs import GenericTimestamp, Limit, T
 from .tuples import Chain
 from .container import Container
 from .coding import BRAID, deletion
```

### Comparing `gink-0.20240601.1717206271/gink/impl/builders.py` & `gink-0.20240601.1717209195/gink/impl/builders.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/impl/bundle_info.py` & `gink-0.20240601.1717209195/gink/impl/bundle_info.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/impl/bundle_store.py` & `gink-0.20240601.1717209195/gink/impl/bundle_store.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 
 from typing import *
 from abc import ABC, abstractmethod
 
+from pathlib import Path
 from .bundle_wrapper import BundleWrapper
 from .tuples import Chain
 from .typedefs import Limit
 from .chain_tracker import ChainTracker
 from .bundle_wrapper import BundleWrapper
+from .watcher import Watcher
 
 class BundleStore(ABC):
     """ Abstract base class for the data store that would serve up data for multiple users. """
 
+    on_ready: Callable  # needs to by dynamically assigned
+
     @abstractmethod
     def apply_bundle(
             self,
             bundle: Union[BundleWrapper, bytes],
             callback: Optional[Callable[[BundleWrapper], None]]=None,
             claim_chain: bool=False) -> bool:
         """ Tries to add data from a particular bundle to this store.
@@ -46,7 +50,38 @@
             The peer_has data can be used to optimize what the store is sending to only what the
             peer needs, but it can be ignored, and it's up to the callback to drop unneeded bundles.
         """
 
     @abstractmethod
     def get_chain_tracker(self, limit_to: Optional[Mapping[Chain, Limit]]=None) -> ChainTracker:
         """Returns a tracker showing what this store has at the time this function is called."""
+
+    @abstractmethod
+    def _get_file_path(self) -> Optional[Path]:
+        """ Return the underlying file name, or None if the store isn't file backed.
+        """
+
+    @abstractmethod
+    def close(self):
+        """ free resources """
+
+    def is_selectable(self) -> bool:
+        return self._get_watcher() is not None
+
+    def _get_watcher(self) -> Optional[Watcher]:
+        if not Watcher.supported():
+            return None
+        file_path = self._get_file_path()
+        if file_path is None:
+            return None
+        if not hasattr(self, "_watcher"):
+            setattr(self, "_watcher", Watcher(file_path))
+        return getattr(self, "_watcher")
+
+    def fileno(self) -> int:
+        watcher = self._get_watcher()
+        assert watcher is not None
+        return watcher.fileno()
+
+    def _clear_notifications(self):
+        if hasattr(self, "_watcher"):
+            self._watcher.clear()
```

### Comparing `gink-0.20240601.1717206271/gink/impl/bundle_wrapper.py` & `gink-0.20240601.1717209195/gink/impl/bundle_wrapper.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/impl/bundler.py` & `gink-0.20240601.1717209195/gink/impl/bundler.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/impl/chain_tracker.py` & `gink-0.20240601.1717209195/gink/impl/chain_tracker.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/impl/coding.py` & `gink-0.20240601.1717209195/gink/impl/coding.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/impl/connection.py` & `gink-0.20240601.1717209195/gink/impl/connection.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/impl/container.py` & `gink-0.20240601.1717209195/gink/impl/container.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/impl/database.py` & `gink-0.20240601.1717209195/gink/impl/database.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,102 +1,69 @@
 #!/usr/bin/env python3
 """ contains the Database class """
 
 # standard python modules
-from typing import Optional, Set, Union, Iterable, List, Callable
-from threading import Lock
+from typing import Optional, Union, Iterable, List
 from sys import stdout
 from logging import getLogger
-from re import fullmatch, IGNORECASE
-from socket import socketpair
+
 
 # builders
 from .builders import ContainerBuilder
 
 # gink modules
 from .abstract_store import AbstractStore
 from .bundler import Bundler
 from .bundle_info import BundleInfo
 from .typedefs import Medallion, MuTimestamp, GenericTimestamp, EPOCH
 from .tuples import Chain
-from .connection import Connection
-from .websocket_connection import WebsocketConnection
-from .listener import Listener
 from .muid import Muid
-from .chain_tracker import ChainTracker
 from .attribution import Attribution
-from .lmdb_store import LmdbStore
-from .memory_store import MemoryStore
 from .bundle_wrapper import BundleWrapper
 from .utilities import (
     generate_timestamp,
     experimental,
     get_identity,
     generate_medallion,
     resolve_timestamp,
 )
-from .looping import Selectable, Finished
+from .relay import Relay
 
-class Database:
+class Database(Relay):
     """ A class that mediates user interaction with a datastore and peers. """
     _chain: Optional[Chain]
-    _lock: Lock
     _last_time: Optional[MuTimestamp]
     _store: AbstractStore
-    _connections: Set[Connection]
-    _listeners: Set[Listener]
-    _sent_but_not_acked: Set[BundleInfo]
     _last_link: Optional[BundleInfo]
     _container_types: dict = {}
 
     def __init__(self, store: Union[AbstractStore, str, None] = None, identity = get_identity()):
+        super().__init__(store=store)
         setattr(Database, "_last", self)
-        if isinstance(store, str):
-            store = LmdbStore(store)
-        if isinstance(store, type(None)):
-            store = MemoryStore()
-        assert isinstance(store, AbstractStore)
-        self._store = store
         self._last_link = None
-        self._lock = Lock()
         self._last_time = None
-        self._connections = set()
-        self._listeners = set()
         self._identity = identity
         self._logger = getLogger(self.__class__.__name__)
-        self._sent_but_not_acked = set()
-        self._callbacks: List[Callable[[BundleInfo], None]] = list()
-        (self._socket_left, self._socket_rite) = socketpair()
-        self._indication_sent = False
-        if self._store.is_selectable():
-            self._indicate_selectables_changed()
-
-    def fileno(self) -> int:
-        return self._socket_rite.fileno()
 
-    @experimental
-    def add_callback(self, callback: Callable[[BundleInfo], None]):
-        self._callbacks.append(callback)
+    def get_store(self) -> AbstractStore:
+        """ returns the store managed by this database """
+        return self._store
 
     @staticmethod
     def get_last():
         last = getattr(Database, "_last")
         assert isinstance(last, Database)
         return last
 
     @classmethod
     def register_container_type(cls, container_cls: type):
         assert hasattr(container_cls, "BEHAVIOR")
         behavior = getattr(container_cls, "BEHAVIOR")
         cls._container_types[behavior] = container_cls
 
-    def get_store(self) -> AbstractStore:
-        """ returns the store managed by this database """
-        return self._store
-
     @experimental
     def get_chain(self) -> Optional[Chain]:
         """ gets the chain this database is appending to (or None if it hasn't started writing yet) """
         if self._last_link is not None:
             return self._last_link.get_chain()
         return None
 
@@ -155,104 +122,14 @@
             added = self._store.apply_bundle(wrap, self._on_bundle, claim_chain=False)
             assert added
             info = wrap.get_info()
             self._last_link = info
             self._logger.debug("locally committed bundle: %r", info)
             return info
 
-    def _on_bundle(self, bundle_wrapper: BundleWrapper) -> None:
-        """ Sends a bundle either created locally or received from a peer to other peers.
-        """
-        for peer in self._connections:
-            peer.send_bundle(bundle_wrapper)
-        for callback in self._callbacks:
-            callback(bundle_wrapper.get_info())
-
-    def _on_connection_ready(self, connection: Connection) -> None:
-        with self._lock:
-            try:
-                for thing in connection.receive_objects():
-                    if isinstance(thing, BundleWrapper):  # some data
-                        self._store.apply_bundle(thing, self._on_bundle)
-                    elif isinstance(thing, ChainTracker):  # greeting message
-                        self._store.get_bundles(connection.send_bundle, peer_has=thing)
-                    elif isinstance(thing, BundleInfo):  # an ack:
-                        self._sent_but_not_acked.discard(thing)
-                    else:
-                        raise AssertionError("unexpected object")
-            except Finished:
-                self._connections.remove(connection)
-                raise
-
-    def _on_listener_ready(self, listener: Listener) -> Iterable[Selectable]:
-        sync_message = self._store.get_chain_tracker().to_greeting_message()
-        connection: Connection = listener.accept(sync_message)
-        connection.on_ready = lambda: self._on_connection_ready(connection)
-        self._connections.add(connection)
-        self._logger.info("accepted incoming connection from %s", connection)
-        return [connection]
-
-    def start_listening(self, ip_addr="", port: Union[str, int] = "8080"):
-        """ Listen for incoming connections on the given port.
-
-            Note that you'll still need to call "run" to actually accept those connections.
-        """
-        port = int(port)
-        self._logger.info("starting to listen on %r:%r", ip_addr, port)
-        listener = Listener(WebsocketConnection, ip_addr=ip_addr, port=port)
-        listener.on_ready = lambda: self._on_listener_ready(listener)
-        self._listeners.add(listener)
-        self._indicate_selectables_changed()
-
-    def connect_to(self, target: str):
-        """ initiate a connection to another gink instance """
-        self._logger.info("initating connection to %s", target)
-        match = fullmatch(r"(ws+://)?([a-z0-9.-]+)(?::(\d+))?(?:/+(.*))?$", target, IGNORECASE)
-        assert match, f"can't connect to: {target}"
-        prefix, host, port, path = match.groups()
-        if prefix and prefix != "ws://":
-            raise NotImplementedError("only vanilla websockets currently supported")
-        port = port or "8080"
-        path = path or "/"
-        greeting = self._store.get_chain_tracker().to_greeting_message()
-        connection = WebsocketConnection(host=host, port=int(port), path=path, greeting=greeting)
-        connection.on_ready = lambda: self._on_connection_ready(connection)
-        self._connections.add(connection)
-        self._logger.debug("connection added")
-        self._indicate_selectables_changed()
-
-    def _on_store_ready(self):
-        self._store.refresh(self._on_bundle)
-
-    def on_ready(self) -> Iterable[Selectable]:
-        if self._indication_sent:
-            self._socket_rite.recv(1)
-            self._indication_sent = False
-        if self._store.is_selectable():
-            self._store.on_ready = self._on_store_ready
-            yield self._store
-        for listener in self._listeners:
-            yield listener
-        for connection in self._connections:
-            yield connection
-
-    def _indicate_selectables_changed(self):
-        if not self._indication_sent:
-            self._socket_left.send(b'0x01')
-            self._indication_sent = True
-
-    def close(self):
-        for connection in self._connections:
-            connection.close()
-        for listener in self._listeners:
-            listener.close()
-        self._store.close()
-        self._socket_left.close()
-        self._socket_rite.close()
-
     def reset(self, to_time: GenericTimestamp = EPOCH, *, bundler=None, comment=None):
         """ Resets the database to a specific point in time.
 
             Note that it literally just "re"-sets everything in one big
             bundle to the values that existed at that time, so you can always
             go and look at the state of the database beforehand.
         """
```

### Comparing `gink-0.20240601.1717206271/gink/impl/deferred.py` & `gink-0.20240601.1717209195/gink/impl/deferred.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/impl/directory.py` & `gink-0.20240601.1717209195/gink/impl/directory.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/impl/graph.py` & `gink-0.20240601.1717209195/gink/impl/graph.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/impl/group.py` & `gink-0.20240601.1717209195/gink/impl/group.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/impl/key_set.py` & `gink-0.20240601.1717209195/gink/impl/key_set.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/impl/listener.py` & `gink-0.20240601.1717209195/gink/impl/listener.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 """ contains the Listener class that listens on a port for incomming connections """
-from typing import Callable, Type
+from typing import Callable, Type, Optional
 from socket import (
     socket as Socket,
     AF_INET,
     SOCK_STREAM,
     SOL_SOCKET,
     SO_REUSEADDR,
 )
 
 from .builders import SyncMessage
 
 from .connection import Connection
 from .websocket_connection import WebsocketConnection
+from .typedefs import AuthFunc
 
 
 class Listener:
     """ Listens on a port for incoming connections. """
 
     on_ready: Callable  # needs to by dynamically assigned
 
-    def __init__(self, connection_class: Type[Connection]=WebsocketConnection, ip_addr: str = "", port: int = 8080):
+    def __init__(
+            self,
+            connection_class: Type[Connection]=WebsocketConnection,
+            ip_addr: str = "",
+            port: int = 8080,
+            auth_func: Optional[AuthFunc] = None,
+            ):
         self._connection_class = connection_class
         self._socket = Socket(AF_INET, SOCK_STREAM)
         self._socket.setsockopt(SOL_SOCKET, SO_REUSEADDR, 1)
         self._socket.bind((ip_addr, int(port)))
         self._socket.listen(128)
+        self._auth_func = auth_func
 
     def fileno(self):
         """ Gives the file descriptor for use in socket.select and similar. """
         return self._socket.fileno()
 
     def close(self):
         self._socket.close()
@@ -36,9 +44,11 @@
     def accept(self, greeting: SyncMessage) -> Connection:
         """ Method to call when the underlying socket is "ready". """
         (new_socket, addr) = self._socket.accept()
         peer: Connection = self._connection_class(
             socket=new_socket,
             host=addr[0],
             port=addr[1],
-            greeting=greeting)
+            greeting=greeting,
+
+            )
         return peer
```

### Comparing `gink-0.20240601.1717206271/gink/impl/lmdb_store.py` & `gink-0.20240601.1717209195/gink/impl/lmdb_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,26 +34,28 @@
 
     def __init__(
             self,
             file_path: Union[str, bytes, Path, None]=None,
             reset=False,
             retain_bundles=True,
             retain_entries=True,
+            apply_changes=True,
             map_size: int=2**30) -> None:
         """ Opens a gink.mdb file for use as a Store.
 
             file_path: where find or place the data file
             reset: if True and file exists, will wipe it after opening
             retain_bundles: if not already set in this file, will specify bundle retention
             retain_entries: if not already set in this file, will specify entry retention
             map_size: Maximum size in bits the database may grow to. Defaults to 1TB
             since there is no penalty for making this number large on 64 bit systems.
         """
         self._logger = getLogger(self.__class__.__name__)
         self._temporary = False
+        self._apply_changes = apply_changes
         if file_path is None:
             prefix = "/tmp/temp."
             if exists("/dev/shm"):
                 prefix = "/dev/shm/temp."
             file_path = prefix + str(uuid.uuid4()) + ".gink.mdb"
             self._temporary = True
         if isinstance(file_path, Path):
@@ -768,14 +770,16 @@
                     trxn.put(bytes(new_info), bundle_location, db=self._bundle_infos)
                 trxn.put(chain_key, bytes(new_info), db=self._chains)
                 change_items: List[int, ChangeBuilder] = list(builder.changes.items())  # type: ignore
                 change_items.sort()  # sometimes the protobuf library doesn't maintain order of maps
                 if new_info.chain_start == new_info.timestamp:
                     trxn.put(bytes(chain_key), new_info.comment.encode())
                 for offset, change in change_items:
+                    if not self._apply_changes:
+                        break
                     try:
                         if change.HasField("container"):
                             trxn.put(bytes(Muid(new_info.timestamp, new_info.medallion, offset)),
                                     change.container.SerializeToString(), db=self._containers)
                             continue
                         if change.HasField("entry"):
                             self._add_entry(new_info, trxn, offset, change.entry)
```

### Comparing `gink-0.20240601.1717206271/gink/impl/lmdb_utilities.py` & `gink-0.20240601.1717209195/gink/impl/lmdb_utilities.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/impl/log_backed_store.py` & `gink-0.20240601.1717209195/gink/impl/log_backed_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/impl/looping.py` & `gink-0.20240601.1717209195/gink/impl/looping.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/impl/memory_store.py` & `gink-0.20240601.1717209195/gink/impl/memory_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/impl/muid.py` & `gink-0.20240601.1717209195/gink/impl/muid.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/impl/pair_map.py` & `gink-0.20240601.1717209195/gink/impl/pair_map.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/impl/pair_set.py` & `gink-0.20240601.1717209195/gink/impl/pair_set.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/impl/property.py` & `gink-0.20240601.1717209195/gink/impl/property.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/impl/selectable_console.py` & `gink-0.20240601.1717209195/gink/impl/selectable_console.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/impl/sequence.py` & `gink-0.20240601.1717209195/gink/impl/sequence.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/impl/tuples.py` & `gink-0.20240601.1717209195/gink/impl/tuples.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/impl/utilities.py` & `gink-0.20240601.1717209195/gink/impl/utilities.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,20 @@
 from datetime import datetime, date, timedelta
 from re import fullmatch
 from psutil import pid_exists
 
 from .typedefs import MuTimestamp, Medallion, GenericTimestamp
 from .tuples import Chain
 from .builders import ClaimBuilder
+from .typedefs import AuthFunc, AUTH_BOTH, AUTH_NONE
+
+def make_auth_func(token: str) -> AuthFunc:
+    def auth_func(data: str) -> int:
+        return AUTH_BOTH if fullmatch(f"token\s+{token}\s*", data, IGNORECASE) else AUTH_NONE
+    return auth_func
 
 def encodeToHex(string: str) -> str:
     """
     Takes a string and encodes it into a hex string prefixed with '0x'.
     """
     # Adding 0x so we can easily determine if a subprotocol is a hex string
     return "0x" + string.encode("utf-8").hex()
```

### Comparing `gink-0.20240601.1717206271/gink/impl/watcher.py` & `gink-0.20240601.1717209195/gink/impl/watcher.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/impl/websocket_connection.py` & `gink-0.20240601.1717209195/gink/impl/websocket_connection.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 
 # batteries included python imports
 from typing import Iterable, Optional, Callable
 from socket import (
     socket as Socket,
     SHUT_WR, SHUT_RDWR
 )
-from select import select
-from os import environ
 
 from .utilities import decodeFromHex, encodeToHex
 
 # modules from requirements.txt
 from wsproto import WSConnection, ConnectionType
 from wsproto.events import (
     Request,
@@ -26,86 +24,82 @@
 
 # builders
 from .builders import SyncMessage
 
 # gink modules
 from .connection import Connection
 from .looping import Finished
+from .typedefs import AuthFunc, AUTH_BOTH
 
 
 class WebsocketConnection(Connection):
     """ Manages the connection to one peer via a websocket.
 
-        Set is_client to indicate that the provided socket is a client connection.
-        If there's no socket provided then one will be established, and is_client is implied.
+        Set force_to_be_client to indicate that the provided socket is a client connection.
+        If there's no socket provided then one will be established, and force_to_be_client is implied.
     """
     PROTOCOL = "gink"
     on_ready: Callable
     def __init__(
             self,
             host: Optional[str] = None,
             port: Optional[int] = None,
             socket: Optional[Socket] = None,
             force_to_be_client: bool = False,
             path: Optional[str] = None,
-            greeting: Optional[SyncMessage] = None
+            greeting: Optional[SyncMessage] = None,
+            auth_func: Optional[AuthFunc] = None,
+            auth_data: Optional[str] = None,
     ):
         Connection.__init__(self, socket=socket, host=host, port=port, greeting=greeting)
         if socket is None:
             force_to_be_client = True
         connection_type = ConnectionType.CLIENT if force_to_be_client else ConnectionType.SERVER
         self._ws = WSConnection(connection_type=connection_type)
         self._ws_closed = False
         self._buffered: bytes = b""
         self._ready = False
-        self.auth_token = environ.get("GINK_AUTH_TOKEN")
         if force_to_be_client:
             subprotocols = [self.PROTOCOL]
-
-            if self.auth_token:
-                assert self.auth_token.lower().startswith("token "), "auth token should start with 'token '"
-                subprotocols.append(encodeToHex(self.auth_token))
-
+            if auth_data:
+                subprotocols.append(encodeToHex(auth_data))
             host = host or "localhost"
             path = path or "/"
             request = Request(host=host, target=path, subprotocols=subprotocols)
             self._socket.send(self._ws.send(request))
         self._logger.debug("finished setup")
         self._socket.settimeout(0.2)
+        self._auth_func = auth_func
+        self._permissions: int = 0 if auth_func else AUTH_BOTH
 
+    def is_alive(self) -> bool:
+        return not (self._ws_closed or self._closed)
 
     def __repr__(self):
         return f"{self.__class__.__name__}(host={self._host!r})"
 
     def receive(self) -> Iterable[SyncMessage]:
         if self._closed:
             raise Finished()
         data = self._socket.recv(4096 * 4096)
         if not data:
             self._ws_closed = True
             raise Finished()
         self._ws.receive_data(data)
         for event in self._ws.events():
             if isinstance(event, Request):
-                if self.auth_token:
-                    # Ensures any capitalization of 'Token' and any number of spaces works
-                    key = self.auth_token.lower().split("token ")[1].lstrip()
-                    token = None
+                if self._auth_func:
                     for protocol in event.subprotocols:
-                        # if we find a hex string in the subprotocols, see if its an auth token
                         if protocol.lower().startswith("0x"):
                             decoded = decodeFromHex(protocol)
-                            if decoded.lower().startswith("token "):
-                                token = decoded.lower().split("token ")[1].lstrip()
-                                break
-                    if not token or token != key:
-                        self._logger.warning("invalid authentication token")
-                        self._socket.send(self._ws.send(RejectConnection()))
-
-                if "gink" not in event.subprotocols:
+                            self._permissions |= self._auth_func(decoded)
+                if not self._permissions:
+                    self._logger.warning("could not authenticated connection")
+                    self._socket.send(self._ws.send(RejectConnection()))
+                elif "gink" not in event.subprotocols:
                     self._logger.warning("got a non gink connection attempt")
                     self._socket.send(self._ws.send(RejectConnection()))
                 else:
                     self._logger.debug("got a Request, sending an AcceptConnection")
                     self._socket.send(self._ws.send(AcceptConnection("gink")))
                     self._logger.info("Server connection established!")
                     self._send_greeting()
```

### Comparing `gink-0.20240601.1717206271/gink/impl/wsgi_connection.py` & `gink-0.20240601.1717209195/gink/impl/wsgi_connection.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/impl/wsgi_listener.py` & `gink-0.20240601.1717209195/gink/impl/wsgi_listener.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/tests/test_box.py` & `gink-0.20240601.1717209195/gink/tests/test_box.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/tests/test_braid.py` & `gink-0.20240601.1717209195/gink/tests/test_braid.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/tests/test_chain_tracker.py` & `gink-0.20240601.1717209195/gink/tests/test_chain_tracker.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/tests/test_change_set_info.py` & `gink-0.20240601.1717209195/gink/tests/test_change_set_info.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/tests/test_code_values.py` & `gink-0.20240601.1717209195/gink/tests/test_code_values.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/tests/test_container.py` & `gink-0.20240601.1717209195/gink/tests/test_container.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/tests/test_database.py` & `gink-0.20240601.1717209195/gink/tests/test_database.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
         db1b = Database(store1b)
 
         root1a = Directory(arche=True, database=db1a)
         root1b = Directory(arche=True, database=db1b)
 
         loop(db1b, until=.01)
         bundle_infos = list()
-        db1b.add_callback(lambda bi: bundle_infos.append(bi))
+        db1b.add_callback(lambda bw: bundle_infos.append(bw.get_info()))
         root1a.set("foo", "bar", comment="abc")
         loop(db1b, until=.01)
         assert bundle_infos and bundle_infos[-1].comment == "abc"
         found = root1b.get("foo")
         assert found == "bar", found
```

### Comparing `gink-0.20240601.1717206271/gink/tests/test_demo.py` & `gink-0.20240601.1717209195/gink/tests/test_demo.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/tests/test_directory.py` & `gink-0.20240601.1717209195/gink/tests/test_directory.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/tests/test_graph.py` & `gink-0.20240601.1717209195/gink/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/tests/test_key_set.py` & `gink-0.20240601.1717209195/gink/tests/test_key_set.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/tests/test_lmdb_store.py` & `gink-0.20240601.1717209195/gink/tests/test_lmdb_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/tests/test_logbackedstore.py` & `gink-0.20240601.1717209195/gink/tests/test_logbackedstore.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/tests/test_muid.py` & `gink-0.20240601.1717209195/gink/tests/test_muid.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/tests/test_names.py` & `gink-0.20240601.1717209195/gink/tests/test_names.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/tests/test_pair_map.py` & `gink-0.20240601.1717209195/gink/tests/test_pair_map.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/tests/test_pair_set.py` & `gink-0.20240601.1717209195/gink/tests/test_pair_set.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/tests/test_property.py` & `gink-0.20240601.1717209195/gink/tests/test_property.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/tests/test_role.py` & `gink-0.20240601.1717209195/gink/tests/test_role.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/tests/test_sequence.py` & `gink-0.20240601.1717209195/gink/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/tests/test_store.py` & `gink-0.20240601.1717209195/gink/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink/tests/test_websocket_connection.py` & `gink-0.20240601.1717209195/gink/tests/test_websocket_connection.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """ tests to make sure that websocket connection works as intended """
 import logging
 from socket import socketpair
 
-import os
-
 # builders
 from ..impl.builders import SyncMessage
 from google.protobuf.text_format import Parse  # type: ignore
 
 from ..impl.websocket_connection import WebsocketConnection, Finished
+from ..impl.utilities import make_auth_func
+from ..impl.looping import loop
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 def test_chit_chat():
     """ ensures that I can send and receive data via a websocket connection """
     server_socket, client_socket = socketpair()
@@ -58,32 +58,50 @@
     except Finished:
         server.close()
 
     assert client.is_closed() and server.is_closed()
 
 def test_auth():
     """ tests authentication """
-    server_socket, client_socket = socketpair()
-
-    os.environ["GINK_AUTH_TOKEN"] = "Token    kjnakjnfakjnfakjnwadhbhbadab"
-    # creating a client connection implicitly sends a request
-    server = WebsocketConnection(socket=server_socket)
-
-    os.environ["GINK_AUTH_TOKEN"] = "Token WRONGAUTHTOKENDONTLETTHROUGH"
-
-    client = WebsocketConnection(socket=client_socket, force_to_be_client=True)
-    getattr(client, "_logger").setLevel(logging.ERROR)
-
-    let_auth_through = False
-    try:
-        # force the server to receive the initial request and send a response
-        for _ in server.receive():
+    for correct in [True, False]:
+        server_socket, client_socket = socketpair()
+        token = "ABCXYZ123"
+        auth_func = make_auth_func(token)
+        # creating a client connection implicitly sends a request
+        server = WebsocketConnection(socket=server_socket, auth_func=auth_func)
+        server.on_ready = lambda: server.receive() and None
+
+        if correct:
+            auth_data = f"Token {token}"
+        else:
+            auth_data = "Token bad"
+
+        client = WebsocketConnection(socket=client_socket, force_to_be_client=True, auth_data=auth_data)
+        client.on_ready = lambda: client.receive() and None
+        getattr(client, "_logger").setLevel(logging.ERROR)
+
+        if correct:
+            loop(server, client, until=.010)
+            assert client.is_alive()
+            assert server.is_alive()
+        else:
+            let_auth_through = False
+            try:
+                # force the server to receive the initial request and send a response
+                loop(server, client, until=.010)
+                assert (not client.is_alive()) and (not server.is_alive())
+                # The above should error when the connection gets rejected,
+                # so let_auth_through should remain false.
+                let_auth_through = True
+            except:
+                pass
+            if let_auth_through:
+                raise AssertionError("auth allowed when token was bad")
+
+        try:
+            server_socket.close()
+            client_socket.close()
+        except:
             pass
-        # The above should error when the connection gets rejected,
-        # so let_auth_through should remain false.
-        let_auth_through = True
-    except:
-        pass
-    assert not let_auth_through, "Server let bad auth token through"
 
 if __name__ == "__main__":
     test_chit_chat()
```

### Comparing `gink-0.20240601.1717206271/gink/tests/test_wsgi_server.py` & `gink-0.20240601.1717209195/gink/tests/test_wsgi_server.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717206271/gink.egg-info/PKG-INFO` & `gink-0.20240601.1717209195/gink.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gink
-Version: 0.20240601.1717206271
+Version: 0.20240601.1717209195
 Summary: a system for storing data structures in lmdb
 Home-page: https://github.com/x5e/gink
 Author: Darin McGill
 Author-email: gink@darinmcgill.com
 Keywords: gink lmdb crdt history versioned
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `gink-0.20240601.1717206271/gink.egg-info/SOURCES.txt` & `gink-0.20240601.1717209195/gink.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 setup.py
 gink/__init__.py
 gink/__main__.py
+gink/braid.py
 gink.egg-info/PKG-INFO
 gink.egg-info/SOURCES.txt
 gink.egg-info/dependency_links.txt
 gink.egg-info/requires.txt
 gink.egg-info/top_level.txt
 gink/builders/__init__.py
 gink/builders/behavior_pb2.py
@@ -26,14 +27,15 @@
 gink/builders/value_pb2.py
 gink/impl/__init__.py
 gink/impl/abstract_store.py
 gink/impl/addressable.py
 gink/impl/attribution.py
 gink/impl/box.py
 gink/impl/braid.py
+gink/impl/braid_server.py
 gink/impl/builders.py
 gink/impl/bundle_info.py
 gink/impl/bundle_store.py
 gink/impl/bundle_wrapper.py
 gink/impl/bundler.py
 gink/impl/chain_tracker.py
 gink/impl/coding.py
@@ -52,14 +54,15 @@
 gink/impl/log_backed_store.py
 gink/impl/looping.py
 gink/impl/memory_store.py
 gink/impl/muid.py
 gink/impl/pair_map.py
 gink/impl/pair_set.py
 gink/impl/property.py
+gink/impl/relay.py
 gink/impl/selectable_console.py
 gink/impl/sequence.py
 gink/impl/tuples.py
 gink/impl/typedefs.py
 gink/impl/utilities.py
 gink/impl/watcher.py
 gink/impl/websocket_connection.py
```

### Comparing `gink-0.20240601.1717206271/setup.py` & `gink-0.20240601.1717209195/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 setup(
     name='gink',
-    version='0.20240601.1717206271',
+    version='0.20240601.1717209195',
     description='a system for storing data structures in lmdb',
     url='https://github.com/x5e/gink',
     author='Darin McGill',
     author_email="gink@darinmcgill.com",
     classifiers=[
         'Development Status :: 4 - Beta',
         "Intended Audience :: Developers",
```

