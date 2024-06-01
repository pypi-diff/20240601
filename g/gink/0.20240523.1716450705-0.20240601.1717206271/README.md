# Comparing `tmp/gink-0.20240523.1716450705.tar.gz` & `tmp/gink-0.20240601.1717206271.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gink-0.20240523.1716450705.tar", last modified: Thu May 23 07:51:50 2024, max compression
+gzip compressed data, was "gink-0.20240601.1717206271.tar", last modified: Sat Jun  1 01:44:34 2024, max compression
```

## Comparing `gink-0.20240523.1716450705.tar` & `gink-0.20240601.1717206271.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:51:50.630248 gink-0.20240523.1716450705/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11194 2024-05-23 07:51:50.630248 gink-0.20240523.1716450705/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9857 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:51:50.614248 gink-0.20240523.1716450705/gink/
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7062 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:51:50.618248 gink-0.20240523.1716450705/gink/builders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 07:51:45.000000 gink-0.20240523.1716450705/gink/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-05-23 07:51:45.000000 gink-0.20240523.1716450705/gink/builders/behavior_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-05-23 07:51:45.000000 gink-0.20240523.1716450705/gink/builders/bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-05-23 07:51:45.000000 gink-0.20240523.1716450705/gink/builders/change_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-23 07:51:45.000000 gink-0.20240523.1716450705/gink/builders/claim_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-05-23 07:51:45.000000 gink-0.20240523.1716450705/gink/builders/clearance_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-23 07:51:45.000000 gink-0.20240523.1716450705/gink/builders/container_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     8918 2024-05-23 07:51:45.000000 gink-0.20240523.1716450705/gink/builders/entry_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-05-23 07:51:45.000000 gink-0.20240523.1716450705/gink/builders/header_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-23 07:51:45.000000 gink-0.20240523.1716450705/gink/builders/key_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-23 07:51:45.000000 gink-0.20240523.1716450705/gink/builders/log_file_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-23 07:51:45.000000 gink-0.20240523.1716450705/gink/builders/movement_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-23 07:51:45.000000 gink-0.20240523.1716450705/gink/builders/muid_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-23 07:51:45.000000 gink-0.20240523.1716450705/gink/builders/pair_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-05-23 07:51:45.000000 gink-0.20240523.1716450705/gink/builders/sync_message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    40439 2024-05-23 07:51:45.000000 gink-0.20240523.1716450705/gink/builders/value_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:51:50.622248 gink-0.20240523.1716450705/gink/impl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11188 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/abstract_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/addressable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/attribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/box.py
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/braid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/builders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/bundle_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/bundle_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/bundle_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/bundler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/chain_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)    19865 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/coding.py
--rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    13325 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/container.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14405 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/deferred.py
--rw-r--r--   0 runner    (1001) docker     (127)    11594 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/directory.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11218 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/key_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/listener.py
--rw-r--r--   0 runner    (1001) docker     (127)    57325 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/lmdb_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/lmdb_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/log_backed_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/looping.py
--rw-r--r--   0 runner    (1001) docker     (127)    23274 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/memory_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/muid.py
--rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/pair_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/pair_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/property.py
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/selectable_console.py
--rw-r--r--   0 runner    (1001) docker     (127)    12612 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/tuples.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/typedefs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/websocket_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/wsgi_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/wsgi_listener.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:51:50.630248 gink-0.20240523.1716450705/gink/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_braid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_chain_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_change_set_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_code_values.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_demo.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10116 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_key_set.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_lmdb_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_logbackedstore.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_memory_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_muid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_pair_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_pair_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_property.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    10500 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    14345 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_websocket_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_wsgi_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:51:50.630248 gink-0.20240523.1716450705/gink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11194 2024-05-23 07:51:50.000000 gink-0.20240523.1716450705/gink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-23 07:51:50.000000 gink-0.20240523.1716450705/gink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 07:51:50.000000 gink-0.20240523.1716450705/gink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-23 07:51:50.000000 gink-0.20240523.1716450705/gink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-23 07:51:50.000000 gink-0.20240523.1716450705/gink.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 07:51:50.630248 gink-0.20240523.1716450705/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-23 07:51:45.000000 gink-0.20240523.1716450705/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:44:34.707765 gink-0.20240601.1717206271/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11216 2024-06-01 01:44:34.707765 gink-0.20240601.1717206271/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9857 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:44:34.691765 gink-0.20240601.1717206271/gink/
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7062 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:44:34.695765 gink-0.20240601.1717206271/gink/builders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 01:44:31.000000 gink-0.20240601.1717206271/gink/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-06-01 01:44:31.000000 gink-0.20240601.1717206271/gink/builders/behavior_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-06-01 01:44:31.000000 gink-0.20240601.1717206271/gink/builders/bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-06-01 01:44:31.000000 gink-0.20240601.1717206271/gink/builders/change_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-06-01 01:44:31.000000 gink-0.20240601.1717206271/gink/builders/claim_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-06-01 01:44:31.000000 gink-0.20240601.1717206271/gink/builders/clearance_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-06-01 01:44:31.000000 gink-0.20240601.1717206271/gink/builders/container_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8918 2024-06-01 01:44:31.000000 gink-0.20240601.1717206271/gink/builders/entry_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-06-01 01:44:31.000000 gink-0.20240601.1717206271/gink/builders/header_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-06-01 01:44:31.000000 gink-0.20240601.1717206271/gink/builders/key_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-06-01 01:44:31.000000 gink-0.20240601.1717206271/gink/builders/log_file_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-06-01 01:44:31.000000 gink-0.20240601.1717206271/gink/builders/movement_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-06-01 01:44:31.000000 gink-0.20240601.1717206271/gink/builders/muid_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-06-01 01:44:31.000000 gink-0.20240601.1717206271/gink/builders/pair_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-06-01 01:44:31.000000 gink-0.20240601.1717206271/gink/builders/sync_message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40439 2024-06-01 01:44:31.000000 gink-0.20240601.1717206271/gink/builders/value_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:44:34.703765 gink-0.20240601.1717206271/gink/impl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11188 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/abstract_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/addressable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/attribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/braid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/bundle_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/bundle_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/bundle_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/bundler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/chain_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19865 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/coding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13325 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/container.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14405 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/deferred.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11594 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11218 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/key_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57325 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/lmdb_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/lmdb_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/log_backed_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/looping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23274 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/memory_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/muid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/pair_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/pair_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/selectable_console.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12612 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/tuples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/typedefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/websocket_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/wsgi_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/impl/wsgi_listener.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:44:34.707765 gink-0.20240601.1717206271/gink/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_braid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_chain_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_change_set_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_code_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_demo.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10116 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_key_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_lmdb_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_logbackedstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_memory_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_muid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_pair_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_pair_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10500 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14345 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_websocket_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-06-01 01:44:18.000000 gink-0.20240601.1717206271/gink/tests/test_wsgi_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:44:34.707765 gink-0.20240601.1717206271/gink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11216 2024-06-01 01:44:34.000000 gink-0.20240601.1717206271/gink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-06-01 01:44:34.000000 gink-0.20240601.1717206271/gink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 01:44:34.000000 gink-0.20240601.1717206271/gink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-06-01 01:44:34.000000 gink-0.20240601.1717206271/gink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-06-01 01:44:34.000000 gink-0.20240601.1717206271/gink.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 01:44:34.707765 gink-0.20240601.1717206271/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-06-01 01:44:31.000000 gink-0.20240601.1717206271/setup.py
```

### Comparing `gink-0.20240523.1716450705/LICENSE` & `gink-0.20240601.1717206271/LICENSE`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/PKG-INFO` & `gink-0.20240601.1717206271/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gink
-Version: 0.20240523.1716450705
+Version: 0.20240601.1717206271
 Summary: a system for storing data structures in lmdb
 Home-page: https://github.com/x5e/gink
 Author: Darin McGill
 Author-email: gink@darinmcgill.com
 Keywords: gink lmdb crdt history versioned
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -17,17 +17,18 @@
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: wsproto
 Requires-Dist: sortedcontainers
 Requires-Dist: lmdb
 Requires-Dist: protobuf<=3.20.3
+Requires-Dist: psutil
 Provides-Extra: test
 Requires-Dist: nose2; extra == "test"
-Requires-Dist: Flask; extra == "test"
+Requires-Dist: flask; extra == "test"
 Requires-Dist: requests; extra == "test"
 Provides-Extra: lint
 Requires-Dist: mypy==0.812; extra == "lint"
 Provides-Extra: performance
 Requires-Dist: matplotlib; extra == "performance"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
```

### Comparing `gink-0.20240523.1716450705/README.md` & `gink-0.20240601.1717206271/README.md`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/__init__.py` & `gink-0.20240601.1717206271/gink/__init__.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/__main__.py` & `gink-0.20240601.1717206271/gink/__main__.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/builders/behavior_pb2.py` & `gink-0.20240601.1717206271/gink/builders/behavior_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/builders/bundle_pb2.py` & `gink-0.20240601.1717206271/gink/builders/bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/builders/change_pb2.py` & `gink-0.20240601.1717206271/gink/builders/change_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/builders/claim_pb2.py` & `gink-0.20240601.1717206271/gink/builders/claim_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/builders/clearance_pb2.py` & `gink-0.20240601.1717206271/gink/builders/clearance_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/builders/container_pb2.py` & `gink-0.20240601.1717206271/gink/builders/container_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/builders/entry_pb2.py` & `gink-0.20240601.1717206271/gink/builders/entry_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/builders/header_pb2.py` & `gink-0.20240601.1717206271/gink/builders/header_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/builders/key_pb2.py` & `gink-0.20240601.1717206271/gink/builders/key_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/builders/log_file_pb2.py` & `gink-0.20240601.1717206271/gink/builders/log_file_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/builders/movement_pb2.py` & `gink-0.20240601.1717206271/gink/builders/movement_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/builders/muid_pb2.py` & `gink-0.20240601.1717206271/gink/builders/muid_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/builders/pair_pb2.py` & `gink-0.20240601.1717206271/gink/builders/pair_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/builders/sync_message_pb2.py` & `gink-0.20240601.1717206271/gink/builders/sync_message_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/builders/value_pb2.py` & `gink-0.20240601.1717206271/gink/builders/value_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/impl/abstract_store.py` & `gink-0.20240601.1717206271/gink/impl/abstract_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/impl/addressable.py` & `gink-0.20240601.1717206271/gink/impl/addressable.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/impl/attribution.py` & `gink-0.20240601.1717206271/gink/impl/attribution.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/impl/box.py` & `gink-0.20240601.1717206271/gink/impl/box.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/impl/braid.py` & `gink-0.20240601.1717206271/gink/impl/braid.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/impl/builders.py` & `gink-0.20240601.1717206271/gink/impl/builders.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/impl/bundle_info.py` & `gink-0.20240601.1717206271/gink/impl/bundle_info.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/impl/bundle_store.py` & `gink-0.20240601.1717206271/gink/impl/bundle_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/impl/bundle_wrapper.py` & `gink-0.20240601.1717206271/gink/impl/bundle_wrapper.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/impl/bundler.py` & `gink-0.20240601.1717206271/gink/impl/bundler.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/impl/chain_tracker.py` & `gink-0.20240601.1717206271/gink/impl/chain_tracker.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/impl/coding.py` & `gink-0.20240601.1717206271/gink/impl/coding.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/impl/connection.py` & `gink-0.20240601.1717206271/gink/impl/connection.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/impl/container.py` & `gink-0.20240601.1717206271/gink/impl/container.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/impl/database.py` & `gink-0.20240601.1717206271/gink/impl/database.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/impl/deferred.py` & `gink-0.20240601.1717206271/gink/impl/deferred.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/impl/directory.py` & `gink-0.20240601.1717206271/gink/impl/directory.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/impl/graph.py` & `gink-0.20240601.1717206271/gink/impl/graph.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/impl/group.py` & `gink-0.20240601.1717206271/gink/impl/group.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/impl/key_set.py` & `gink-0.20240601.1717206271/gink/impl/key_set.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/impl/listener.py` & `gink-0.20240601.1717206271/gink/impl/listener.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/impl/lmdb_store.py` & `gink-0.20240601.1717206271/gink/impl/lmdb_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/impl/lmdb_utilities.py` & `gink-0.20240601.1717206271/gink/impl/lmdb_utilities.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/impl/log_backed_store.py` & `gink-0.20240601.1717206271/gink/impl/log_backed_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/impl/looping.py` & `gink-0.20240601.1717206271/gink/impl/looping.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/impl/memory_store.py` & `gink-0.20240601.1717206271/gink/impl/memory_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/impl/muid.py` & `gink-0.20240601.1717206271/gink/impl/muid.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/impl/pair_map.py` & `gink-0.20240601.1717206271/gink/impl/pair_map.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/impl/pair_set.py` & `gink-0.20240601.1717206271/gink/impl/pair_set.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/impl/property.py` & `gink-0.20240601.1717206271/gink/impl/property.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/impl/selectable_console.py` & `gink-0.20240601.1717206271/gink/impl/selectable_console.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/impl/sequence.py` & `gink-0.20240601.1717206271/gink/impl/sequence.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/impl/tuples.py` & `gink-0.20240601.1717206271/gink/impl/tuples.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/impl/typedefs.py` & `gink-0.20240601.1717206271/gink/impl/typedefs.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/impl/utilities.py` & `gink-0.20240601.1717206271/gink/impl/utilities.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from time import time as get_time, sleep
 from math import floor
 from os import getuid, getpid
-from os.path import exists
 from socket import gethostname
 from pwd import getpwuid
 from functools import wraps
 from warnings import warn
 from random import randint
-from platform import system
 from datetime import datetime, date, timedelta
-from re import fullmatch, IGNORECASE
+from re import fullmatch
+from psutil import pid_exists
 
 from .typedefs import MuTimestamp, Medallion, GenericTimestamp
 from .tuples import Chain
 from .builders import ClaimBuilder
 
 def encodeToHex(string: str) -> str:
     """
@@ -70,17 +69,16 @@
     if the_class:
         the_class.__init__ = wrapped
         return the_class
     else:
         return wrapped
 
 def is_certainly_gone(process_id: int) -> bool:
-    if system() == 'Linux' and exists("/proc") and not exists("/proc/%s" % process_id):
+    if not pid_exists(process_id):
         return True
-    # TODO(https://github.com/x5e/gink/issues/203) figure out a solution for macos
     return False
 
 def create_claim(chain: Chain) -> ClaimBuilder:
     claim_builder = ClaimBuilder()
     claim_builder.claim_time = generate_timestamp()
     claim_builder.medallion = chain.medallion
     claim_builder.chain_start = chain.chain_start
```

### Comparing `gink-0.20240523.1716450705/gink/impl/watcher.py` & `gink-0.20240601.1717206271/gink/impl/watcher.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/impl/websocket_connection.py` & `gink-0.20240601.1717206271/gink/impl/websocket_connection.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/impl/wsgi_connection.py` & `gink-0.20240601.1717206271/gink/impl/wsgi_connection.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/impl/wsgi_listener.py` & `gink-0.20240601.1717206271/gink/impl/wsgi_listener.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/tests/test_box.py` & `gink-0.20240601.1717206271/gink/tests/test_box.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/tests/test_braid.py` & `gink-0.20240601.1717206271/gink/tests/test_braid.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/tests/test_chain_tracker.py` & `gink-0.20240601.1717206271/gink/tests/test_chain_tracker.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/tests/test_change_set_info.py` & `gink-0.20240601.1717206271/gink/tests/test_change_set_info.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/tests/test_code_values.py` & `gink-0.20240601.1717206271/gink/tests/test_code_values.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/tests/test_container.py` & `gink-0.20240601.1717206271/gink/tests/test_container.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/tests/test_database.py` & `gink-0.20240601.1717206271/gink/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/tests/test_demo.py` & `gink-0.20240601.1717206271/gink/tests/test_demo.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/tests/test_directory.py` & `gink-0.20240601.1717206271/gink/tests/test_directory.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/tests/test_graph.py` & `gink-0.20240601.1717206271/gink/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/tests/test_key_set.py` & `gink-0.20240601.1717206271/gink/tests/test_key_set.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/tests/test_lmdb_store.py` & `gink-0.20240601.1717206271/gink/tests/test_lmdb_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/tests/test_logbackedstore.py` & `gink-0.20240601.1717206271/gink/tests/test_logbackedstore.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/tests/test_muid.py` & `gink-0.20240601.1717206271/gink/tests/test_muid.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/tests/test_names.py` & `gink-0.20240601.1717206271/gink/tests/test_names.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/tests/test_pair_map.py` & `gink-0.20240601.1717206271/gink/tests/test_pair_map.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/tests/test_pair_set.py` & `gink-0.20240601.1717206271/gink/tests/test_pair_set.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/tests/test_property.py` & `gink-0.20240601.1717206271/gink/tests/test_property.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/tests/test_role.py` & `gink-0.20240601.1717206271/gink/tests/test_role.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/tests/test_sequence.py` & `gink-0.20240601.1717206271/gink/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/tests/test_store.py` & `gink-0.20240601.1717206271/gink/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/tests/test_websocket_connection.py` & `gink-0.20240601.1717206271/gink/tests/test_websocket_connection.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink/tests/test_wsgi_server.py` & `gink-0.20240601.1717206271/gink/tests/test_wsgi_server.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/gink.egg-info/PKG-INFO` & `gink-0.20240601.1717206271/gink.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gink
-Version: 0.20240523.1716450705
+Version: 0.20240601.1717206271
 Summary: a system for storing data structures in lmdb
 Home-page: https://github.com/x5e/gink
 Author: Darin McGill
 Author-email: gink@darinmcgill.com
 Keywords: gink lmdb crdt history versioned
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -17,17 +17,18 @@
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: wsproto
 Requires-Dist: sortedcontainers
 Requires-Dist: lmdb
 Requires-Dist: protobuf<=3.20.3
+Requires-Dist: psutil
 Provides-Extra: test
 Requires-Dist: nose2; extra == "test"
-Requires-Dist: Flask; extra == "test"
+Requires-Dist: flask; extra == "test"
 Requires-Dist: requests; extra == "test"
 Provides-Extra: lint
 Requires-Dist: mypy==0.812; extra == "lint"
 Provides-Extra: performance
 Requires-Dist: matplotlib; extra == "performance"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
```

### Comparing `gink-0.20240523.1716450705/gink.egg-info/SOURCES.txt` & `gink-0.20240601.1717206271/gink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gink-0.20240523.1716450705/setup.py` & `gink-0.20240601.1717206271/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 setup(
     name='gink',
-    version='0.20240523.1716450705',
+    version='0.20240601.1717206271',
     description='a system for storing data structures in lmdb',
     url='https://github.com/x5e/gink',
     author='Darin McGill',
     author_email="gink@darinmcgill.com",
     classifiers=[
         'Development Status :: 4 - Beta',
         "Intended Audience :: Developers",
@@ -22,17 +22,18 @@
     packages=find_packages(),
     python_requires=">=3.8, <4",
     install_requires=[
         "wsproto",
         "sortedcontainers",
         "lmdb",
         "protobuf<=3.20.3",
+        "psutil"
     ],
     extras_require={
-        "test": ["nose2", "Flask", "requests"],
+        "test": ["nose2", "flask", "requests"],
         "lint": ["mypy==0.812"],
         "performance": ["matplotlib"],
         "docs": [
             "sphinx",
             "myst-parser",
             "sphinx-rtd-theme",
             "sphinx-copybutton"
```

