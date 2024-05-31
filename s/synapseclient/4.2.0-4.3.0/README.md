# Comparing `tmp/synapseclient-4.2.0.tar.gz` & `tmp/synapseclient-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synapseclient-4.2.0.tar", last modified: Fri Apr 19 00:44:54 2024, max compression
+gzip compressed data, was "synapseclient-4.3.0.tar", last modified: Fri May 31 23:40:11 2024, max compression
```

## Comparing `synapseclient-4.2.0.tar` & `synapseclient-4.3.0.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:44:54.906554 synapseclient-4.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-19 00:44:41.000000 synapseclient-4.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14561 2024-04-19 00:44:54.906554 synapseclient-4.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10823 2024-04-19 00:44:41.000000 synapseclient-4.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-19 00:44:41.000000 synapseclient-4.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-19 00:44:54.906554 synapseclient-4.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-19 00:44:41.000000 synapseclient-4.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:44:54.886554 synapseclient-4.2.0/synapseclient/
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/.synapseConfig
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    63395 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13315 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/activity.py
--rw-r--r--   0 runner    (1001) docker     (127)    17293 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/annotations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:44:54.890554 synapseclient-4.2.0/synapseclient/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/api/annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/api/entity_bundle_services_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6158 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/api/entity_services.py
--rw-r--r--   0 runner    (1001) docker     (127)    12946 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/api/file_services.py
--rw-r--r--   0 runner    (1001) docker     (127)   254964 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:44:54.890554 synapseclient-4.2.0/synapseclient/core/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/async_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    19498 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:44:54.890554 synapseclient-4.2.0/synapseclient/core/constants/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/constants/concrete_types.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/constants/config_file_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/constants/limits.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/constants/method_flags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:44:54.894554 synapseclient-4.2.0/synapseclient/core/credentials/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/credentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/credentials/cred_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    10919 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/credentials/credential_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/cumulative_transfer_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/dozer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9570 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/logging_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:44:54.894554 synapseclient-4.2.0/synapseclient/core/models/
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/models/custom_json.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/models/dict_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     8257 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/models/permission.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:44:54.894554 synapseclient-4.2.0/synapseclient/core/multithread_download/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/multithread_download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15712 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/multithread_download/download_threads.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/pool_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    13171 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/remote_file_storage_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)    22468 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)    10815 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/sts_transfer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:44:54.894554 synapseclient-4.2.0/synapseclient/core/upload/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24662 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/upload/multipart_upload.py
--rw-r--r--   0 runner    (1001) docker     (127)    30626 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/upload/multipart_upload_async.py
--rw-r--r--   0 runner    (1001) docker     (127)    13110 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/upload/upload_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    15164 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/upload/upload_functions_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/upload/upload_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    45377 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/version_check.py
--rw-r--r--   0 runner    (1001) docker     (127)    34756 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     9581 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/evaluation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:44:54.894554 synapseclient-4.2.0/synapseclient/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14489 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)    51831 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/file.py
--rw-r--r--   0 runner    (1001) docker     (127)    19293 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/folder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:44:54.898554 synapseclient-4.2.0/synapseclient/models/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/mixins/access_control.py
--rw-r--r--   0 runner    (1001) docker     (127)    16436 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/mixins/storable_container.py
--rw-r--r--   0 runner    (1001) docker     (127)    20794 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:44:54.898554 synapseclient-4.2.0/synapseclient/models/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/protocols/access_control_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/protocols/activity_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/protocols/annotations_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    10340 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/protocols/file_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/protocols/folder_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/protocols/project_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/protocols/storable_container_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/protocols/table_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/protocols/team_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/protocols/user_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:44:54.898554 synapseclient-4.2.0/synapseclient/models/services/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/services/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/services/storable_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     7653 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/services/storable_entity_components.py
--rw-r--r--   0 runner    (1001) docker     (127)    29342 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/table.py
--rw-r--r--   0 runner    (1001) docker     (127)    14168 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/team.py
--rw-r--r--   0 runner    (1001) docker     (127)    13651 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/user.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/wiki.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:44:54.898554 synapseclient-4.2.0/synapseclient/services/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28756 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/services/json_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-19 00:44:42.000000 synapseclient-4.2.0/synapseclient/synapsePythonClient
--rw-r--r--   0 runner    (1001) docker     (127)    94315 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/team.py
--rw-r--r--   0 runner    (1001) docker     (127)     5284 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/wiki.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:44:54.898554 synapseclient-4.2.0/synapseclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14561 2024-04-19 00:44:54.000000 synapseclient-4.2.0/synapseclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-04-19 00:44:54.000000 synapseclient-4.2.0/synapseclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 00:44:54.000000 synapseclient-4.2.0/synapseclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-19 00:44:54.000000 synapseclient-4.2.0/synapseclient.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 00:44:48.000000 synapseclient-4.2.0/synapseclient.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-19 00:44:54.000000 synapseclient-4.2.0/synapseclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-19 00:44:54.000000 synapseclient-4.2.0/synapseclient.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:44:54.898554 synapseclient-4.2.0/synapseutils/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37471 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseutils/copy_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseutils/describe_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    53640 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseutils/migrate_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseutils/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    53640 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseutils/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseutils/walk_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:40:11.853319 synapseclient-4.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-31 23:39:59.000000 synapseclient-4.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15262 2024-05-31 23:40:11.853319 synapseclient-4.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11412 2024-05-31 23:39:59.000000 synapseclient-4.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-31 23:39:59.000000 synapseclient-4.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-31 23:40:11.853319 synapseclient-4.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-31 23:39:59.000000 synapseclient-4.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:40:11.837319 synapseclient-4.3.0/synapseclient/
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/.synapseConfig
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63334 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13315 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17293 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/annotations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:40:11.837319 synapseclient-4.3.0/synapseclient/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/api/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/api/entity_bundle_services_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/api/entity_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12946 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/api/file_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)   255620 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:40:11.841319 synapseclient-4.3.0/synapseclient/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/core/async_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19513 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/core/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/core/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:40:11.841319 synapseclient-4.3.0/synapseclient/core/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/core/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/core/constants/concrete_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/core/constants/config_file_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/core/constants/limits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/core/constants/method_flags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:40:11.841319 synapseclient-4.3.0/synapseclient/core/credentials/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/core/credentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/core/credentials/cred_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10919 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/core/credentials/credential_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/core/cumulative_transfer_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/core/dozer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9570 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/core/lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/core/logging_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:40:11.841319 synapseclient-4.3.0/synapseclient/core/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/core/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/core/models/custom_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/core/models/dict_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8257 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/core/models/permission.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:40:11.841319 synapseclient-4.3.0/synapseclient/core/multithread_download/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/core/multithread_download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15712 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/core/multithread_download/download_threads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/core/pool_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13171 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/core/remote_file_storage_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22708 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/core/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10815 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/core/sts_transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:40:11.841319 synapseclient-4.3.0/synapseclient/core/upload/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/core/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24662 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/core/upload/multipart_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31436 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/core/upload/multipart_upload_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13110 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/core/upload/upload_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15164 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/core/upload/upload_functions_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/core/upload/upload_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45597 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/core/version_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34756 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9581 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:40:11.845319 synapseclient-4.3.0/synapseclient/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15665 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/models/activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/models/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/models/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56469 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/models/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19293 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/models/folder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:40:11.845319 synapseclient-4.3.0/synapseclient/models/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/models/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/models/mixins/access_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16525 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/models/mixins/storable_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20794 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/models/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:40:11.845319 synapseclient-4.3.0/synapseclient/models/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/models/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/models/protocols/access_control_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/models/protocols/activity_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/models/protocols/annotations_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10340 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/models/protocols/file_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/models/protocols/folder_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/models/protocols/project_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/models/protocols/storable_container_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/models/protocols/table_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/models/protocols/team_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/models/protocols/user_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:40:11.845319 synapseclient-4.3.0/synapseclient/models/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/models/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/models/services/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/models/services/storable_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9246 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/models/services/storable_entity_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30031 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/models/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14168 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/models/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13651 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/models/wiki.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:40:11.849319 synapseclient-4.3.0/synapseclient/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28756 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/services/json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/synapsePythonClient
+-rw-r--r--   0 runner    (1001) docker     (127)    94315 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5284 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseclient/wiki.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:40:11.849319 synapseclient-4.3.0/synapseclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15262 2024-05-31 23:40:11.000000 synapseclient-4.3.0/synapseclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-31 23:40:11.000000 synapseclient-4.3.0/synapseclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 23:40:11.000000 synapseclient-4.3.0/synapseclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-31 23:40:11.000000 synapseclient-4.3.0/synapseclient.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 23:40:05.000000 synapseclient-4.3.0/synapseclient.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-31 23:40:11.000000 synapseclient-4.3.0/synapseclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-31 23:40:11.000000 synapseclient-4.3.0/synapseclient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:40:11.849319 synapseclient-4.3.0/synapseutils/
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37471 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseutils/copy_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseutils/describe_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53640 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseutils/migrate_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6595 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseutils/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56903 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseutils/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-05-31 23:39:59.000000 synapseclient-4.3.0/synapseutils/walk_functions.py
```

### Comparing `synapseclient-4.2.0/PKG-INFO` & `synapseclient-4.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synapseclient
-Version: 4.2.0
+Version: 4.3.0
 Summary: A client for Synapse, a collaborative, open-source research platform that allows teams to share data, track analyses, and collaborate.
 Home-page: https://www.synapse.org
 Author: The Synapse Engineering Team
 Author-email: platform@sagebase.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/Sage-Bionetworks/synapsePythonClient
 Project-URL: Tracker, https://github.com/Sage-Bionetworks/synapsePythonClient/issues
@@ -39,35 +39,37 @@
 Requires-Dist: asyncio-atexit~=1.0.1
 Requires-Dist: httpx~=0.27.0
 Requires-Dist: tqdm<5.0,>=4.66.2
 Requires-Dist: loky~=3.0.0
 Requires-Dist: async-lru~=2.0.4
 Requires-Dist: psutil~=5.9.8
 Provides-Extra: dev
-Requires-Dist: pytest<7.0,>=6.0.0; extra == "dev"
+Requires-Dist: pytest<8.0,>=7.0.0; extra == "dev"
 Requires-Dist: pytest-mock<4.0,>=3.0; extra == "dev"
 Requires-Dist: pytest-socket~=0.6.0; extra == "dev"
-Requires-Dist: pytest-asyncio~=0.19; extra == "dev"
+Requires-Dist: pytest-asyncio<1.0,>=0.23.6; extra == "dev"
 Requires-Dist: flake8<4.0,>=3.7.0; extra == "dev"
 Requires-Dist: pytest-xdist[psutil]<3.0.0,>=2.2; extra == "dev"
 Requires-Dist: pytest-rerunfailures~=12.0; extra == "dev"
 Requires-Dist: func-timeout~=4.3; extra == "dev"
 Requires-Dist: pytest-cov~=4.1.0; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pandas<3.0,>=1.5; extra == "dev"
 Provides-Extra: tests
-Requires-Dist: pytest<7.0,>=6.0.0; extra == "tests"
+Requires-Dist: pytest<8.0,>=7.0.0; extra == "tests"
 Requires-Dist: pytest-mock<4.0,>=3.0; extra == "tests"
 Requires-Dist: pytest-socket~=0.6.0; extra == "tests"
-Requires-Dist: pytest-asyncio~=0.19; extra == "tests"
+Requires-Dist: pytest-asyncio<1.0,>=0.23.6; extra == "tests"
 Requires-Dist: flake8<4.0,>=3.7.0; extra == "tests"
 Requires-Dist: pytest-xdist[psutil]<3.0.0,>=2.2; extra == "tests"
 Requires-Dist: pytest-rerunfailures~=12.0; extra == "tests"
 Requires-Dist: func-timeout~=4.3; extra == "tests"
 Requires-Dist: pytest-cov~=4.1.0; extra == "tests"
+Requires-Dist: pandas<3.0,>=1.5; extra == "tests"
 Provides-Extra: pandas
 Requires-Dist: pandas<3.0,>=1.5; extra == "pandas"
 Provides-Extra: pysftp
 Requires-Dist: pysftp<0.3,>=0.2.8; extra == "pysftp"
 Provides-Extra: boto3
 Requires-Dist: boto3<2.0,>=1.7.0; extra == "boto3"
 Provides-Extra: docs
@@ -121,33 +123,48 @@
 
 **Starting from Synapse Python client version 3.0, Synapse Python client requires Python >= 3.8**
 
 ### Install using pip
 
 The [Python Synapse Client is on PyPI](https://pypi.python.org/pypi/synapseclient) and can be installed with pip:
 
-    (sudo) pip install synapseclient[pandas,pysftp]
+    # Here are a few ways to install the client. Choose the one that fits your use-case
+    # sudo may optionally be needed depending on your setup
+
+    pip install --upgrade synapseclient
+    pip install --upgrade "synapseclient[pandas]"
+    pip install --upgrade "synapseclient[pandas, pysftp, boto3]"
 
 ...or to upgrade an existing installation of the Synapse client:
 
-    (sudo) pip install --upgrade synapseclient
+    # sudo may optionally be needed depending on your setup
+    pip install --upgrade synapseclient
 
-The dependencies on `pandas` and `pysftp` are optional. Synapse [Tables](https://python-docs.synapse.org/reference/tables/) integrate
+The dependencies on `pandas`, `pysftp`, and `boto3` are optional. Synapse
+[Tables](https://python-docs.synapse.org/reference/tables/) integrate
 with [Pandas](http://pandas.pydata.org/). The library `pysftp` is required for users of
-[SFTP](https://python-docs.synapse.org/guides/data_storage/#sftp) file storage. Both libraries require native code
-to be compiled or installed separately from prebuilt binaries.
+[SFTP](https://python-docs.synapse.org/guides/data_storage/#sftp) file storage. All
+libraries require native code to be compiled or installed separately from prebuilt
+binaries.
 
 ### Install from source
 
 Clone the [source code repository](https://github.com/Sage-Bionetworks/synapsePythonClient).
 
     git clone git://github.com/Sage-Bionetworks/synapsePythonClient.git
     cd synapsePythonClient
     pip install .
 
+Alternatively, you can use pip to install a particular branch, commit, or other git reference:
+
+    pip install git+https://github.com/Sage-Bionetworks/synapsePythonClient@master
+
+or
+
+    pip install git+https://github.com/Sage-Bionetworks/synapsePythonClient@my-commit-hash
 
 Command line usage
 ------------------
 
 The Synapse client can be used from the shell command prompt. Valid commands
 include: query, get, cat, add, update, delete, and onweb. A few examples are
 shown.
```

### Comparing `synapseclient-4.2.0/README.md` & `synapseclient-4.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -40,33 +40,48 @@
 
 **Starting from Synapse Python client version 3.0, Synapse Python client requires Python >= 3.8**
 
 ### Install using pip
 
 The [Python Synapse Client is on PyPI](https://pypi.python.org/pypi/synapseclient) and can be installed with pip:
 
-    (sudo) pip install synapseclient[pandas,pysftp]
+    # Here are a few ways to install the client. Choose the one that fits your use-case
+    # sudo may optionally be needed depending on your setup
+
+    pip install --upgrade synapseclient
+    pip install --upgrade "synapseclient[pandas]"
+    pip install --upgrade "synapseclient[pandas, pysftp, boto3]"
 
 ...or to upgrade an existing installation of the Synapse client:
 
-    (sudo) pip install --upgrade synapseclient
+    # sudo may optionally be needed depending on your setup
+    pip install --upgrade synapseclient
 
-The dependencies on `pandas` and `pysftp` are optional. Synapse [Tables](https://python-docs.synapse.org/reference/tables/) integrate
+The dependencies on `pandas`, `pysftp`, and `boto3` are optional. Synapse
+[Tables](https://python-docs.synapse.org/reference/tables/) integrate
 with [Pandas](http://pandas.pydata.org/). The library `pysftp` is required for users of
-[SFTP](https://python-docs.synapse.org/guides/data_storage/#sftp) file storage. Both libraries require native code
-to be compiled or installed separately from prebuilt binaries.
+[SFTP](https://python-docs.synapse.org/guides/data_storage/#sftp) file storage. All
+libraries require native code to be compiled or installed separately from prebuilt
+binaries.
 
 ### Install from source
 
 Clone the [source code repository](https://github.com/Sage-Bionetworks/synapsePythonClient).
 
     git clone git://github.com/Sage-Bionetworks/synapsePythonClient.git
     cd synapsePythonClient
     pip install .
 
+Alternatively, you can use pip to install a particular branch, commit, or other git reference:
+
+    pip install git+https://github.com/Sage-Bionetworks/synapsePythonClient@master
+
+or
+
+    pip install git+https://github.com/Sage-Bionetworks/synapsePythonClient@my-commit-hash
 
 Command line usage
 ------------------
 
 The Synapse client can be used from the shell command prompt. Valid commands
 include: query, get, cat, add, update, delete, and onweb. A few examples are
 shown.
```

### Comparing `synapseclient-4.2.0/setup.cfg` & `synapseclient-4.3.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -48,47 +48,50 @@
 	asyncio-atexit~=1.0.1
 	httpx~=0.27.0
 	tqdm>=4.66.2,<5.0
 	loky~=3.0.0
 	async-lru~=2.0.4
 	psutil~=5.9.8
 tests_require = 
-	pytest>=6.0.0,<7.0
+	pytest>=7.0.0,<8.0
 	pytest-mock>=3.0,<4.0
 	pytest-socket~=0.6.0
-	pytest-asyncio~=0.19
+	pytest-asyncio>=0.23.6,<1.0
 	flake8>=3.7.0,<4.0
 	pytest-xdist[psutil]>=2.2,<3.0.0
 	pytest-rerunfailures~=12.0
 	func-timeout~=4.3
 	pytest-cov~=4.1.0
+	pandas>=1.5,<3.0
 
 [options.extras_require]
 dev = 
-	pytest>=6.0.0,<7.0
+	pytest>=7.0.0,<8.0
 	pytest-mock>=3.0,<4.0
 	pytest-socket~=0.6.0
-	pytest-asyncio~=0.19
+	pytest-asyncio>=0.23.6,<1.0
 	flake8>=3.7.0,<4.0
 	pytest-xdist[psutil]>=2.2,<3.0.0
 	pytest-rerunfailures~=12.0
 	func-timeout~=4.3
 	pytest-cov~=4.1.0
 	black
 	pre-commit
+	pandas>=1.5,<3.0
 tests = 
-	pytest>=6.0.0,<7.0
+	pytest>=7.0.0,<8.0
 	pytest-mock>=3.0,<4.0
 	pytest-socket~=0.6.0
-	pytest-asyncio~=0.19
+	pytest-asyncio>=0.23.6,<1.0
 	flake8>=3.7.0,<4.0
 	pytest-xdist[psutil]>=2.2,<3.0.0
 	pytest-rerunfailures~=12.0
 	func-timeout~=4.3
 	pytest-cov~=4.1.0
+	pandas>=1.5,<3.0
 pandas = 
 	pandas>=1.5,<3.0
 pysftp = 
 	pysftp>=0.2.8,<0.3
 boto3 = 
 	boto3>=1.7.0,<2.0
 docs =
```

### Comparing `synapseclient-4.2.0/setup.py` & `synapseclient-4.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/.synapseConfig` & `synapseclient-4.3.0/synapseclient/.synapseConfig`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/__init__.py` & `synapseclient-4.3.0/synapseclient/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -84,12 +84,17 @@
 ]
 
 USER_AGENT = {
     "User-Agent": "synapseclient/%s %s"
     % (__version__, requests.utils.default_user_agent())
 }
 
+USER_AGENT_COMMAND_LINE = {
+    "User-Agent": "synapsecommandlineclient/%s %s"
+    % (__version__, requests.utils.default_user_agent())
+}
+
 # patch json
 from .core.models import custom_json  # noqa
 
 # patch logging
 from .core import logging_setup  # noqa
```

### Comparing `synapseclient-4.2.0/synapseclient/__main__.py` & `synapseclient-4.3.0/synapseclient/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1867,17 +1867,15 @@
         # otherwise if none of them applied then a no credentials error
         # will result in a login prompt
         raise first_auth_ex or SynapseNoCredentialsError()
 
 
 def main():
     args = build_parser().parse_args()
-    synapseclient.USER_AGENT["User-Agent"] = (
-        "synapsecommandlineclient " + synapseclient.USER_AGENT["User-Agent"]
-    )
+    synapseclient.USER_AGENT = synapseclient.USER_AGENT_COMMAND_LINE
     if args.otel:
         trace.set_tracer_provider(
             TracerProvider(
                 sampler=ParentBased(ALWAYS_ON),
                 resource=Resource(attributes={SERVICE_NAME: "synapseclient"}),
             )
         )
```

### Comparing `synapseclient-4.2.0/synapseclient/activity.py` & `synapseclient-4.3.0/synapseclient/activity.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/annotations.py` & `synapseclient-4.3.0/synapseclient/annotations.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/api/__init__.py` & `synapseclient-4.3.0/synapseclient/api/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from .entity_services import (
     get_entity,
     get_upload_destination,
     get_upload_destination_location,
     post_entity,
     put_entity,
     create_access_requirements_if_none,
+    delete_entity_generated_by,
 )
 from .file_services import (
     get_file_handle,
     post_external_filehandle,
     post_external_object_store_filehandle,
     post_external_s3_file_handle,
     post_file_multipart,
@@ -47,8 +48,9 @@
     # entity_services
     "get_entity",
     "put_entity",
     "post_entity",
     "get_upload_destination",
     "get_upload_destination_location",
     "create_access_requirements_if_none",
+    "delete_entity_generated_by",
 ]
```

### Comparing `synapseclient-4.2.0/synapseclient/api/annotations.py` & `synapseclient-4.3.0/synapseclient/api/annotations.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/api/entity_bundle_services_v2.py` & `synapseclient-4.3.0/synapseclient/api/entity_bundle_services_v2.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/api/entity_services.py` & `synapseclient-4.3.0/synapseclient/api/entity_services.py`

 * *Files 9% similar despite different names*

```diff
@@ -171,7 +171,27 @@
         )
         client.logger.info(
             "Created an access requirements request for "
             f"{entity_id}: {access_requirements['jiraKey']}. An email will be sent to "
             "the Synapse access control team to start the process of adding "
             "terms-of-use or review board approval for this entity."
         )
+
+
+async def delete_entity_generated_by(
+    entity_id: str,
+    synapse_client: Optional["Synapse"] = None,
+) -> None:
+    """
+    Arguments:
+        entity_id: The ID of the entity.
+        synapse_client: If not passed in or None this will use the last client from
+            the `.login()` method.
+
+    Returns: None
+    """
+    from synapseclient import Synapse
+
+    client = Synapse.get_client(synapse_client=synapse_client)
+    return await client.rest_delete_async(
+        uri=f"/entity/{entity_id}/generatedBy",
+    )
```

### Comparing `synapseclient-4.2.0/synapseclient/api/file_services.py` & `synapseclient-4.3.0/synapseclient/api/file_services.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/client.py` & `synapseclient-4.3.0/synapseclient/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,30 +117,26 @@
 )
 from synapseclient.core import sts_transfer
 from synapseclient.core.upload.multipart_upload_async import (
     multipart_upload_file_async,
     multipart_upload_string_async,
 )
 from synapseclient.core.remote_file_storage_wrappers import S3ClientWrapper, SFTPWrapper
-from synapseclient.core.upload.upload_functions import (
-    upload_file_handle,
-)
 from synapseclient.core.upload.upload_functions_async import (
     upload_file_handle as upload_file_handle_async,
     upload_synapse_s3,
 )
 from synapseclient.core.dozer import doze
 from synapseclient.core.async_utils import wrap_async_to_sync
 
 from typing import Any, Union, Dict, List, Optional, Tuple
 from synapseclient.core.models.permission import Permissions
 from opentelemetry import trace
 from opentelemetry.trace import SpanKind
 
-
 tracer = trace.get_tracer("synapseclient")
 
 PRODUCTION_ENDPOINTS = {
     "repoEndpoint": "https://repo-prod.prod.sagebase.org/repo/v1",
     "authEndpoint": "https://auth-prod.prod.sagebase.org/auth/v1",
     "fileHandleEndpoint": "https://file-prod.prod.sagebase.org/file/v1",
     "portalEndpoint": "https://www.synapse.org/",
@@ -344,15 +340,15 @@
             """
             span = span_dict.pop(response.request, None)
             if span and span.is_recording():
                 span.set_attribute("http.response.status_code", response.status_code)
                 span.end()
 
         event_hooks = {"request": [log_request], "response": [log_response]}
-        httpx_timeout = httpx.Timeout(70)
+        httpx_timeout = httpx.Timeout(70, pool=None)
         self._requests_session_storage = requests_session_storage or httpx.Client(
             timeout=httpx_timeout, event_hooks=event_hooks
         )
 
         cache_root_dir = (
             cache.CACHE_ROOT_DIR if cache_root_dir is None else cache_root_dir
         )
@@ -398,14 +394,15 @@
         self.table_query_timeout = 600  # in seconds
         self.multi_threaded = True  # if set to True, multi threaded download will be used for http and https URLs
 
         transfer_config = self._get_transfer_config()
         self.max_threads = transfer_config["max_threads"]
         self._thread_executor = {}
         self._process_executor = {}
+        self._parallel_file_transfer_semaphore = {}
         self._md5_semaphore = {}
         self.use_boto_sts_transfers = transfer_config["use_boto_sts"]
 
     def _get_requests_session_async_synapse(
         self, asyncio_event_loop: asyncio.AbstractEventLoop
     ) -> httpx.AsyncClient:
         """
@@ -431,15 +428,15 @@
             return self._requests_session_async_synapse[asyncio_event_loop]
 
         async def close_connection() -> None:
             """Close connection when event loop exits"""
             await self._requests_session_async_synapse[asyncio_event_loop].aclose()
             del self._requests_session_async_synapse[asyncio_event_loop]
 
-        httpx_timeout = httpx.Timeout(70)
+        httpx_timeout = httpx.Timeout(70, pool=None)
         span_dict: Dict[httpx.Request, trace.Span] = {}
 
         async def log_request(request: httpx.Request) -> None:
             """
             Log the HTTPX request to an otel span.
 
             Arguments:
@@ -558,14 +555,53 @@
         ):
             return self._md5_semaphore[asyncio_event_loop]
 
         self._md5_semaphore.update({asyncio_event_loop: asyncio.Semaphore(1)})
 
         return self._md5_semaphore[asyncio_event_loop]
 
+    def _get_parallel_file_transfer_semaphore(
+        self, asyncio_event_loop: asyncio.AbstractEventLoop
+    ) -> asyncio.Semaphore:
+        """
+        Retrieve the semaphore for the Synapse client. Or create a new one if it does
+        not exist. This semaphore is used to limit the number of files that can actively
+        enter the uploading/downloading process.
+
+        This is expected to be called from within an AsyncIO loop.
+
+        By default the number of files that can enter the "uploading" state will be
+        limited to 2 * max_threads. This is to ensure that the files that are entering
+        into the "uploading" state will have priority to finish. Additionally, it means
+        that there should be a good spread of files getting up to the "uploading"
+        state, entering the "uploading" state, and finishing the "uploading" state.
+
+        If we break these states down into large components they would look like:
+        - Before "uploading" state: HTTP rest calls to retrieve what data Synapse has
+        - Entering "uploading" state: MD5 calculation and HTTP rest calls to determine
+          how/where to upload a file to.
+        - During "uploading" state: Uploading the file to a storage provider.
+        - After "uploading" state: HTTP rest calls to finalize the upload.
+
+        This has not yet been applied to parallel file downloads. That will take place
+        later on.
+        """
+        if (
+            hasattr(self, "_parallel_file_transfer_semaphore")
+            and asyncio_event_loop in self._parallel_file_transfer_semaphore
+            and self._parallel_file_transfer_semaphore[asyncio_event_loop] is not None
+        ):
+            return self._parallel_file_transfer_semaphore[asyncio_event_loop]
+
+        self._parallel_file_transfer_semaphore.update(
+            {asyncio_event_loop: asyncio.Semaphore(max(self.max_threads * 2, 1))}
+        )
+
+        return self._parallel_file_transfer_semaphore[asyncio_event_loop]
+
     # initialize logging
     def _init_logger(self):
         """
         Initialize logging
         """
         logger_name = (
             SILENT_LOGGER_NAME
@@ -712,18 +748,18 @@
         Valid combinations of login() arguments:
 
         - authToken
 
         If no login arguments are provided or only username is provided, login() will attempt to log in using
          information from these sources (in order of preference):
 
-        1. User defined arguments during a CLI session
-        2. User's Personal Access Token (aka: Synapse Auth Token)
+        1. .synapseConfig file (in user home folder unless configured otherwise)
+        2. User defined arguments during a CLI session
+        3. User's Personal Access Token (aka: Synapse Auth Token)
             from the environment variable: SYNAPSE_AUTH_TOKEN
-        3. .synapseConfig file (in user home folder unless configured otherwise)
         4. Retrieves user's authentication token from AWS SSM Parameter store (if configured)
 
         Arguments:
             email:        Synapse user name (or an email address associated with a Synapse account)
             authToken:    A bearer authorization token, e.g. a
                 [personal access token](https://python-docs.synapse.org/tutorials/authentication/).
             silent:       Defaults to False.  Suppresses the "Welcome ...!" message.
@@ -1725,15 +1761,14 @@
         isRestricted=False,
         activity=None,
         used=None,
         executed=None,
         activityName=None,
         activityDescription=None,
         set_annotations=True,
-        async_file_handle_upload: bool = True,
     ):
         """
         Creates a new Entity or updates an existing Entity, uploading any files in the process.
 
         Arguments:
             obj: A Synapse Entity, Evaluation, or Wiki
             used: The Entity, Synapse ID, or URL used to create the object (can also be a list of these)
@@ -1748,19 +1783,14 @@
                             has changed.
             versionLabel: Arbitrary string used to label the version.
             isRestricted: If set to true, an email will be sent to the Synapse access control team to start the
                             process of adding terms-of-use or review board approval for this entity.
                             You will be contacted with regards to the specific data being restricted and the
                             requirements of access.
             set_annotations: If True, set the annotations on the entity. If False, do not set the annotations.
-            async_file_handle_upload: Temporary feature flag that will be removed at an
-                unannounced later date. This is used during the Synapse Utils
-                syncToSynapse to disable the async file handle upload. The is because
-                the multi-threaded logic in the syncToSynapse is not compatible with
-                the async file handle upload.
 
         Returns:
             A Synapse Entity, Evaluation, or Wiki
 
         Example: Using this function
             Creating a new Project:
 
@@ -1912,45 +1942,28 @@
                     parent_id_for_upload = bundle["entity"]["parentId"]
 
                 if not parent_id_for_upload:
                     raise SynapseMalformedEntityError(
                         "Entities of type File must have a parentId."
                     )
 
-                if async_file_handle_upload:
-                    fileHandle = wrap_async_to_sync(
-                        upload_file_handle_async(
-                            self,
-                            parent_id_for_upload,
-                            local_state["path"]
-                            if (
-                                synapseStore
-                                or local_state_fh.get("externalURL") is None
-                            )
-                            else local_state_fh.get("externalURL"),
-                            synapse_store=synapseStore,
-                            md5=local_file_md5_hex or local_state_fh.get("contentMd5"),
-                            file_size=local_state_fh.get("contentSize"),
-                            mimetype=local_state_fh.get("contentType"),
-                        ),
-                        self,
-                    )
-                else:
-                    fileHandle = upload_file_handle(
+                fileHandle = wrap_async_to_sync(
+                    upload_file_handle_async(
                         self,
                         parent_id_for_upload,
                         local_state["path"]
                         if (synapseStore or local_state_fh.get("externalURL") is None)
                         else local_state_fh.get("externalURL"),
-                        synapseStore=synapseStore,
+                        synapse_store=synapseStore,
                         md5=local_file_md5_hex or local_state_fh.get("contentMd5"),
                         file_size=local_state_fh.get("contentSize"),
                         mimetype=local_state_fh.get("contentType"),
-                        max_threads=self.max_threads,
-                    )
+                    ),
+                    self,
+                )
                 properties["dataFileHandleId"] = fileHandle["id"]
                 local_state["_file_handle"] = fileHandle
 
             elif "dataFileHandleId" not in properties:
                 # Handle the case where the Entity lacks an ID
                 # But becomes an update() due to conflict
                 properties["dataFileHandleId"] = bundle["entity"]["dataFileHandleId"]
@@ -6023,15 +6036,14 @@
                 if isinstance(data, str):
                     data_to_parse = data
                 elif isinstance(data, bytes):
                     data_to_parse = data.decode("utf-8")
                 else:
                     return
                 data_dict = json.loads(data_to_parse)
-
                 if "parentId" in data_dict:
                     current_span.set_attribute(
                         "synapse.parent_id", data_dict["parentId"]
                     )
                 if "id" in data_dict:
                     current_span.set_attribute("synapse.id", data_dict["id"])
                 if "concreteType" in data_dict:
```

### Comparing `synapseclient-4.2.0/synapseclient/core/async_utils.py` & `synapseclient-4.3.0/synapseclient/core/async_utils.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/core/cache.py` & `synapseclient-4.3.0/synapseclient/core/cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
     def __setattr__(self, key, value):
         # expand out home shortcut ('~') and environment variables when setting cache_root_dir
         if key == "cache_root_dir":
             value = os.path.expandvars(os.path.expanduser(value))
             # create the cache_root_dir if it does not already exist
             if not os.path.exists(value):
-                os.makedirs(value)
+                os.makedirs(value, exist_ok=True)
         self.__dict__[key] = value
 
     def __init__(self, cache_root_dir=CACHE_ROOT_DIR, fanout=1000):
         # set root dir of cache in which meta data will be stored and files
         # will be stored here by default, but other locations can be specified
         self.cache_root_dir = cache_root_dir
         self.fanout = fanout
```

### Comparing `synapseclient-4.2.0/synapseclient/core/constants/concrete_types.py` & `synapseclient-4.3.0/synapseclient/core/constants/concrete_types.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/core/credentials/cred_data.py` & `synapseclient-4.3.0/synapseclient/core/credentials/cred_data.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/core/credentials/credential_provider.py` & `synapseclient-4.3.0/synapseclient/core/credentials/credential_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,17 +205,17 @@
     [SynapseCredentialsProvider][synapseclient.core.credentials.credential_provider.SynapseCredentialsProvider]
     from which this class attempts to retrieve
     [SynapseCredentials][synapseclient.core.credentials.cred_data.SynapseCredentials].
 
 
     By default this class uses the following providers in this order:
 
-    1. [UserArgsCredentialsProvider][synapseclient.core.credentials.credential_provider.UserArgsCredentialsProvider]
-    2. [EnvironmentVariableCredentialsProvider][synapseclient.core.credentials.credential_provider.EnvironmentVariableCredentialsProvider]
-    3. [ConfigFileCredentialsProvider][synapseclient.core.credentials.credential_provider.ConfigFileCredentialsProvider]
+    1. [ConfigFileCredentialsProvider][synapseclient.core.credentials.credential_provider.ConfigFileCredentialsProvider]
+    2. [UserArgsCredentialsProvider][synapseclient.core.credentials.credential_provider.UserArgsCredentialsProvider]
+    3. [EnvironmentVariableCredentialsProvider][synapseclient.core.credentials.credential_provider.EnvironmentVariableCredentialsProvider]
     4. [AWSParameterStoreCredentialsProvider][synapseclient.core.credentials.credential_provider.AWSParameterStoreCredentialsProvider]
 
     Attributes:
         cred_providers: list of
             ([SynapseCredentialsProvider][synapseclient.core.credentials.credential_provider.SynapseCredentialsProvider])
             credential providers
     """
```

### Comparing `synapseclient-4.2.0/synapseclient/core/cumulative_transfer_progress.py` & `synapseclient-4.3.0/synapseclient/core/cumulative_transfer_progress.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/core/dozer.py` & `synapseclient-4.3.0/synapseclient/core/dozer.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/core/exceptions.py` & `synapseclient-4.3.0/synapseclient/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/core/lock.py` & `synapseclient-4.3.0/synapseclient/core/lock.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/core/logging_setup.py` & `synapseclient-4.3.0/synapseclient/core/logging_setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -92,10 +92,20 @@
             },
             DEBUG_LOGGER_NAME: {
                 "handlers": ["info_only_stdout", "debug_stderr"],
                 "level": "DEBUG",
                 "propagate": True,
             },
             SILENT_LOGGER_NAME: {"handlers": [], "level": "INFO", "propagate": False},
+            # "httpx": {
+            #     "handlers": ["debug_stderr"],
+            #     "level": "DEBUG",
+            #     "propagate": True,
+            # },
+            # "httpcore": {
+            #     "handlers": ["debug_stderr"],
+            #     "level": "DEBUG",
+            #     "propagate": True,
+            # },
         },
     }
 )
```

### Comparing `synapseclient-4.2.0/synapseclient/core/models/custom_json.py` & `synapseclient-4.3.0/synapseclient/core/models/custom_json.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/core/models/dict_object.py` & `synapseclient-4.3.0/synapseclient/core/models/dict_object.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/core/models/permission.py` & `synapseclient-4.3.0/synapseclient/core/models/permission.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/core/multithread_download/download_threads.py` & `synapseclient-4.3.0/synapseclient/core/multithread_download/download_threads.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/core/pool_provider.py` & `synapseclient-4.3.0/synapseclient/core/pool_provider.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/core/remote_file_storage_wrappers.py` & `synapseclient-4.3.0/synapseclient/core/remote_file_storage_wrappers.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/core/retry.py` & `synapseclient-4.3.0/synapseclient/core/retry.py`

 * *Files 1% similar despite different names*

```diff
@@ -324,14 +324,16 @@
     # Retry until we succeed or run past the maximum wait time
     total_wait = 0
     retries = -1
     while True:
         caught_exception = None
         caught_exception_info = None
         response = None
+        current_span = trace.get_current_span()
+        current_span.set_attribute("synapse.retries", str(retries + 1))
 
         try:
             response = await function()
         except Exception as ex:
             caught_exception = ex
             caught_exception_info = sys.exc_info()
             logger.debug(DEBUG_EXCEPTION, function, exc_info=True)
@@ -445,14 +447,16 @@
     # Retry until we succeed or run past the maximum wait time
     total_wait = 0
     retries = -1
     while True:
         caught_exception = None
         caught_exception_info = None
         response = None
+        current_span = trace.get_current_span()
+        current_span.set_attribute("synapse.retries", str(retries + 1))
 
         try:
             response = function()
         except Exception as ex:
             caught_exception = ex
             caught_exception_info = sys.exc_info()
             logger.debug(DEBUG_EXCEPTION, function, exc_info=True)
```

### Comparing `synapseclient-4.2.0/synapseclient/core/sts_transfer.py` & `synapseclient-4.3.0/synapseclient/core/sts_transfer.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/core/upload/__init__.py` & `synapseclient-4.3.0/synapseclient/core/upload/__init__.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/core/upload/multipart_upload.py` & `synapseclient-4.3.0/synapseclient/core/upload/multipart_upload.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/core/upload/multipart_upload_async.py` & `synapseclient-4.3.0/synapseclient/core/upload/multipart_upload_async.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 
     post-upload --> entity["Create/Update Synapse entity"]
 ```
 """
 
 # pylint: disable=protected-access
 import asyncio
+from contextlib import contextmanager
 import gc
 import mimetypes
 import os
 import threading
 from dataclasses import dataclass
 from typing import (
     TYPE_CHECKING,
@@ -122,14 +123,30 @@
 MAX_NUMBER_OF_PARTS = 10000
 MIN_PART_SIZE = 5 * MB
 
 # ancient tribal knowledge
 DEFAULT_PART_SIZE = 8 * MB
 MAX_RETRIES = 7
 
+_thread_local = threading.local()
+
+
+@contextmanager
+def shared_progress_bar(progress_bar):
+    """An outside process that will eventually trigger an upload through this module
+    can configure a shared Progress Bar by running its code within this context manager.
+    """
+    _thread_local.progress_bar = progress_bar
+    try:
+        yield
+    finally:
+        _thread_local.progress_bar.close()
+        _thread_local.progress_bar.refresh()
+        del _thread_local.progress_bar
+
 
 @dataclass
 class HandlePartResult:
     """Result of a part upload.
 
     Attributes:
         part_number: The part number that was uploaded.
@@ -169,14 +186,15 @@
         self._force_restart = force_restart
 
         self._lock = asyncio.Lock()
         self._thread_lock = threading.Lock()
         self._aborted = False
         self._storage_str = storage_str
 
+        self._close_progress_bar = getattr(_thread_local, "progress_bar", None) is None
         # populated later
         self._upload_id: Optional[str] = None
         self._pre_signed_part_urls: Optional[Mapping[int, str]] = None
         self._progress_bar = None
 
     async def __call__(self) -> Dict[str, str]:
         """Orchestrate the upload of a file to Synapse."""
@@ -325,29 +343,33 @@
                 asyncio.create_task(self._handle_part_wrapper(part_number=part_number))
             )
 
         if not self._syn.silent and not self._progress_bar:
             if self._is_copy():
                 # we won't have bytes to measure during a copy so the byte oriented
                 # progress bar is not useful
-                self._progress_bar = tqdm(
+                self._progress_bar = getattr(
+                    _thread_local, "progress_bar", None
+                ) or tqdm(
                     total=part_count,
                     desc=self._storage_str or "Copying",
                     unit_scale=True,
                     postfix=self._dest_file_name,
                     smoothing=0,
                 )
                 self._progress_bar.update(completed_part_count)
             else:
                 previously_transferred = min(
                     completed_part_count * self._part_size,
                     file_size,
                 )
 
-                self._progress_bar = tqdm(
+                self._progress_bar = getattr(
+                    _thread_local, "progress_bar", None
+                ) or tqdm(
                     total=file_size,
                     desc=self._storage_str or "Uploading",
                     unit="B",
                     unit_scale=True,
                     postfix=self._dest_file_name,
                     smoothing=0,
                 )
@@ -444,15 +466,15 @@
 
     async def _complete_upload(self) -> Dict[str, str]:
         """Close the upload and mark it as complete.
 
         Returns:
             The response from the server for the completed upload.
         """
-        if not self._syn.silent and self._progress_bar:
+        if not self._syn.silent and self._progress_bar and self._close_progress_bar:
             self._progress_bar.close()
         upload_status_response = await put_file_multipart_complete(
             upload_id=self._upload_id,
             endpoint=self._syn.fileHandleEndpoint,
             synapse_client=self._syn,
         )
```

### Comparing `synapseclient-4.2.0/synapseclient/core/upload/upload_functions.py` & `synapseclient-4.3.0/synapseclient/core/upload/upload_functions.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/core/upload/upload_functions_async.py` & `synapseclient-4.3.0/synapseclient/core/upload/upload_functions_async.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/core/upload/upload_utils.py` & `synapseclient-4.3.0/synapseclient/core/upload/upload_utils.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/core/utils.py` & `synapseclient-4.3.0/synapseclient/core/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1396,34 +1396,38 @@
         for key in list(incoming_object.keys()):
             if incoming_object[key] is None:
                 del incoming_object[key]
 
 
 def merge_dataclass_entities(
     source: typing.Union["Project", "Folder", "File"],
-    destination: typing.Union["Project", "Folder"],
-) -> typing.Union["Project", "Folder"]:
+    destination: typing.Union["Project", "Folder", "File"],
+    fields_to_ignore: typing.List[str] = None,
+) -> typing.Union["Project", "Folder", "File"]:
     """
     Utility function to merge two dataclass entities together. This is used when we are
     upserting an entity from the Synapse service with the requested changes.
 
     Arguments:
         source: The source entity to merge from.
         destination: The destination entity to merge into.
+        fields_to_ignore: A list of fields to ignore when merging.
 
     Returns:
         The destination entity with the merged values.
     """
     # Convert dataclasses to dictionaries
     destination_dict = asdict(destination)
     source_dict = asdict(source)
     modified_items = {}
 
     # Update destination_dict with source_dict, keeping destination's values in case of conflicts
     for key, value in source_dict.items():
+        if fields_to_ignore is not None and key in fields_to_ignore:
+            continue
         if is_dataclass(getattr(source, key)):
             if hasattr(destination, key):
                 setattr(destination, key, getattr(source, key))
             else:
                 modified_items[key] = merge_dataclass_entities(
                     getattr(source, key), destination=getattr(destination, key)
                 )
```

### Comparing `synapseclient-4.2.0/synapseclient/core/version_check.py` & `synapseclient-4.3.0/synapseclient/core/version_check.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/entity.py` & `synapseclient-4.3.0/synapseclient/entity.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/evaluation.py` & `synapseclient-4.3.0/synapseclient/evaluation.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/models/__init__.py` & `synapseclient-4.3.0/synapseclient/models/__init__.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/models/activity.py` & `synapseclient-4.3.0/synapseclient/models/activity.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import asyncio
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, Dict, List, NamedTuple, Optional, Union
 
 from opentelemetry import context, trace
 
 from synapseclient import Synapse
+from synapseclient.api import delete_entity_generated_by
 from synapseclient.activity import Activity as Synapse_Activity
 from synapseclient.core.async_utils import async_to_sync, otel_trace_method
 from synapseclient.core.constants.concrete_types import USED_ENTITY, USED_URL
 from synapseclient.core.exceptions import SynapseHTTPError
 from synapseclient.core.utils import run_and_attach_otel_context
 from synapseclient.models.protocols.activity_protocol import ActivitySynchronousProtocol
 
@@ -385,7 +386,36 @@
                         synapse_client=synapse_client
                     ).deleteProvenance(
                         entity=parent.id,
                     ),
                     current_context,
                 ),
             )
+            parent.activity = None
+
+    @classmethod
+    async def disassociate_from_entity_async(
+        cls,
+        parent: Union["Table", "File"],
+        synapse_client: Optional[Synapse] = None,
+    ) -> None:
+        """
+        Disassociate the Activity from the parent entity. This is the first step in
+        deleting the Activity. If you have other entities that are associated with this
+        Activity you must disassociate them by calling this method on them as well.
+
+        Arguments:
+            parent: The parent entity this activity is associated with.
+            synapse_client: If not passed in or None this will use the last client
+                from the `.login()` method.
+
+        Raises:
+            ValueError: If the parent does not have an ID.
+        """
+        # TODO: Input validation: SYNPY-1400
+        with tracer.start_as_current_span(
+            name=f"Activity_disassociate: Parent_ID: {parent.id}"
+        ):
+            await delete_entity_generated_by(
+                entity_id=parent.id, synapse_client=synapse_client
+            )
+            parent.activity = None
```

### Comparing `synapseclient-4.2.0/synapseclient/models/annotations.py` & `synapseclient-4.3.0/synapseclient/models/annotations.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/models/file.py` & `synapseclient-4.3.0/synapseclient/models/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 from synapseclient.models.mixins.access_control import AccessControllable
 from synapseclient.models.protocols.file_protocol import FileSynchronousProtocol
 from synapseclient.models.services.search import get_id
 from synapseclient.models.services.storable_entity import store_entity
 from synapseclient.models.services.storable_entity_components import (
     store_entity_components,
 )
-from synapseutils.copy_functions import changeFileMetaData, copy
 
 if TYPE_CHECKING:
     from synapseclient.models import Folder, Project
 
 
 @dataclass()
 class FileHandle:
@@ -195,15 +194,18 @@
             have permission to store the file.
         external_url: The external URL of this file. If this is set AND `synapse_store`
             is False, only a reference to this URL and the file metadata will be stored
             in Synapse. The file itself will not be uploaded. If this attribute is set
             it will override the `path`.
         activity: The Activity model represents the main record of Provenance in
             Synapse. It is analygous to the Activity defined in the
-            [W3C Specification](https://www.w3.org/TR/prov-n/) on Provenance.
+            [W3C Specification](https://www.w3.org/TR/prov-n/) on Provenance. Activity
+            cannot be removed during a store operation by setting it to None. You must
+            use: [synapseclient.models.Activity.delete_async][] or
+            [synapseclient.models.Activity.disassociate_from_entity_async][].
         annotations: Additional metadata associated with the folder. The key is the name
             of your desired annotations. The value is an object containing a list of
             values (use empty list to represent no values for key) and the value type
             associated with all values in the list. To remove all annotations set this
             to an empty dict `{}` or None and store the entity.
 
     Attributes:
@@ -231,30 +233,43 @@
             read from synapse use the `.file_handle.content_md5` attribute.
         create_or_update: (Store only)
             Indicates whether the method should automatically perform an
             update if the `file` conflicts with an existing Synapse object.
         force_version: (Store only)
             Indicates whether the method should increment the version of the object if
             something within the entity has changed. For example updating the
-            description or annotations. You may set this to False and an update to the
+            description or name. You may set this to False and an update to the
             entity will not increment the version.
 
             Updating the `version_label` attribute will also cause a version update
             regardless  of this flag.
 
             An update to the MD5 of the file will force a version update regardless of
             this  flag.
         is_restricted: (Store only)
             If set to true, an email will be sent to the Synapse access control
             team to start the process of adding terms-of-use or review board approval
             for this entity. You will be contacted with regards to the specific data
             being restricted and the requirements of access.
 
             This may be used only by an administrator of the specified file.
-
+        merge_existing_annotations: (Store only)
+            Works in conjunction with `create_or_update` in that this is only evaluated
+            if `create_or_update` is True. If this entity exists in Synapse that has
+            annotations that are not present in a store operation, these annotations
+            will be added to the entity. If this is False any annotations that are not
+            present within a store operation will be removed from this entity. This
+            allows one to complete a destructive update of annotations on an entity.
+        associate_activity_to_new_version: (Store only)
+            Works in conjunction with `create_or_update` in that this is only evaluated
+            if `create_or_update` is True. When true an activity already attached to the
+            current version of this entity will be associated the new version during a
+            store operation if the version was updated. This is useful if you are
+            updating the entity and want to ensure that the activity is persisted onto
+            the new version the entity.
         synapse_store: (Store only)
             Whether the File should be uploaded or if false: only the path should
             be stored when [synapseclient.models.File.store][] is called.
 
     Attributes:
         download_file: (Get only) If True the file will be downloaded.
         download_location: (Get only) The location to download the file to.
@@ -328,15 +343,19 @@
     a reference to this URL and the file metadata will be stored in Synapse. The file
     itself will not be uploaded. If this attribute is set it will override the `path`.
     """
 
     activity: Optional[Activity] = field(default=None, compare=False)
     """The Activity model represents the main record of Provenance in Synapse.  It is
     analygous to the Activity defined in the
-    [W3C Specification](https://www.w3.org/TR/prov-n/) on Provenance."""
+    [W3C Specification](https://www.w3.org/TR/prov-n/) on Provenance. Activity cannot
+    be removed during a store operation by setting it to None. You must use:
+    [synapseclient.models.Activity.delete_async][] or
+    [synapseclient.models.Activity.disassociate_from_entity_async][].
+    """
 
     annotations: Optional[
         Dict[
             str,
             Union[
                 List[str],
                 List[bool],
@@ -392,15 +411,15 @@
     """
 
     force_version: bool = field(default=True, repr=False, compare=False)
     """
     (Store only)
 
     Indicates whether the method should increment the version of the object if something
-    within the entity has changed. For example updating the description or annotations.
+    within the entity has changed. For example updating the description or name.
     You may set this to False and an update to the entity will not increment the
     version.
 
     Updating the `version_label` attribute will also cause a version update regardless
     of this flag.
 
     An update to the MD5 of the file will force a version update regardless of this
@@ -415,14 +434,49 @@
     the process of adding terms-of-use or review board approval for this entity.
     You will be contacted with regards to the specific data being restricted and the
     requirements of access.
 
     This may be used only by an administrator of the specified file.
     """
 
+    merge_existing_annotations: bool = field(default=True, repr=False, compare=False)
+    """
+    (Store only)
+
+    Works in conjunction with `create_or_update` in that this is only evaluated if
+    `create_or_update` is True. If this entity exists in Synapse that has annotations
+    that are not present in a store operation, these annotations will be added to the
+    entity. If this is False any annotations that are not present within a store
+    operation will be removed from this entity. This allows one to complete a
+    destructive update of annotations on an entity.
+    """
+
+    associate_activity_to_new_version: bool = field(
+        default=False, repr=False, compare=False
+    )
+    """
+    (Store only)
+
+    Works in conjunction with `create_or_update` in that this is only evaluated if
+    `create_or_update` is True. When true an activity already attached to the current
+    version of this entity will be associated the new version during a store operation
+    if the version was updated. This is useful if you are updating the entity and want
+    to ensure that the activity is persisted onto the new version the entity.
+
+    When this is False the activity will not be associated to the new version of the
+    entity during a store operation.
+
+    Regardless of this setting, if you have an Activity object on the entity it will be
+    persisted onto the new version. This is only used when you don't have an Activity
+    object on the entity.
+    """
+
+    _present_manifest_fields: List[str] = field(default=None, repr=False, compare=False)
+    """Hidden attribute to pass along what columns were present in a manifest upload."""
+
     synapse_store: bool = field(default=True, repr=False)
     """
     (Store only)
 
     Whether the File should be uploaded or if false: only the path should be stored when
     [synapseclient.models.File.store][] is called.
     """
@@ -612,15 +666,17 @@
                 file_copy = File(
                     id=existing_id,
                     download_file=False,
                     version_number=self.version_number,
                     synapse_container_limit=self.synapse_container_limit,
                     parent_id=self.parent_id,
                 )
-                return await file_copy.get_async(synapse_client=synapse_client)
+                return await file_copy.get_async(
+                    synapse_client=synapse_client, include_activity=True
+                )
             except SynapseFileNotFoundError:
                 return None
 
         if (
             self.create_or_update
             and not self._last_persistent_instance
             and (
@@ -631,14 +687,39 @@
                 )
             )
             and (existing_file := await get_file(existing_file_id))
         ):
             return existing_file
         return None
 
+    def _determine_fields_to_ignore_in_merge(self) -> List[str]:
+        """This is used to determine what fields should not be merged when merging two
+        entities. This allows for a fine tuned destructive update of an entity.
+
+        This also has special handling during a manifest upload of files. If a manifest
+        is specifying fields we'll use those values rather than copying them from the
+        existing entity. This is to allow for a destructive update of an entity.
+
+        """
+        fields_to_not_merge = []
+        if not self.merge_existing_annotations:
+            fields_to_not_merge.append("annotations")
+
+        if not self.associate_activity_to_new_version:
+            fields_to_not_merge.append("activity")
+
+        if self._present_manifest_fields:
+            if "name" in self._present_manifest_fields:
+                fields_to_not_merge.append("name")
+
+            if "contentType" in self._present_manifest_fields:
+                fields_to_not_merge.append("content_type")
+
+        return fields_to_not_merge
+
     @otel_trace_method(
         method_to_trace_name=lambda self, **kwargs: f"File_Store: {self.path if self.path else self.id}"
     )
     async def store_async(
         self,
         parent: Optional[Union["Folder", "Project"]] = None,
         synapse_client: Optional[Synapse] = None,
@@ -719,19 +800,26 @@
                 "(path with a (`parent_id` or parent with an id)), or a "
                 "(data_file_handle_id with a (`parent_id` or parent with an id)) to store."
             )
         self.name = self.name or (guess_file_name(self.path) if self.path else None)
         client = Synapse.get_client(synapse_client=synapse_client)
 
         if existing_file := await self._find_existing_file(synapse_client=client):
-            merge_dataclass_entities(source=existing_file, destination=self)
+            merge_dataclass_entities(
+                source=existing_file,
+                destination=self,
+                fields_to_ignore=self._determine_fields_to_ignore_in_merge(),
+            )
 
         if self.path:
             self.path = os.path.expanduser(self.path)
-            await self._upload_file(synapse_client=client)
+            async with client._get_parallel_file_transfer_semaphore(
+                asyncio_event_loop=asyncio.get_running_loop()
+            ):
+                await self._upload_file(synapse_client=client)
         elif self.data_file_handle_id:
             self.path = client.cache.get(file_handle_id=self.data_file_handle_id)
 
         if self.has_changed:
             synapse_file = Synapse_File(
                 id=self.id,
                 path=self.path,
@@ -810,14 +898,15 @@
                 print(file_entity.name) ## prints, "my_new_name_file.txt"
 
         Raises:
             ValueError: If the file does not have an ID to change metadata.
         """
         if not self.id:
             raise ValueError("The file must have an ID to change metadata.")
+        from synapseutils.copy_functions import changeFileMetaData
 
         loop = asyncio.get_event_loop()
 
         current_context = context.get_current()
         syn = Synapse.get_client(synapse_client=synapse_client)
         entity = await loop.run_in_executor(
             None,
@@ -1081,14 +1170,15 @@
                 new_file_instance = await File(id="syn123").copy_async(parent_id="syn456", copy_annotations=False, copy_activity=None)
 
         Raises:
             ValueError: If the file does not have an ID and parent_id to copy.
         """
         if not self.id or not parent_id:
             raise ValueError("The file must have an ID and parent_id to copy.")
+        from synapseutils.copy_functions import copy
 
         loop = asyncio.get_event_loop()
 
         current_context = context.get_current()
         syn = Synapse.get_client(synapse_client=synapse_client)
         source_and_destination = await loop.run_in_executor(
             None,
```

### Comparing `synapseclient-4.2.0/synapseclient/models/folder.py` & `synapseclient-4.3.0/synapseclient/models/folder.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/models/mixins/access_control.py` & `synapseclient-4.3.0/synapseclient/models/mixins/access_control.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/models/mixins/storable_container.py` & `synapseclient-4.3.0/synapseclient/models/mixins/storable_container.py`

 * *Files 1% similar despite different names*

```diff
@@ -367,15 +367,19 @@
             file = File(id=synapse_id, name=name, download_file=download_file)
             self.files.append(file)
             if path:
                 file.download_location = path
             if if_collision:
                 file.if_collision = if_collision
 
-            pending_tasks.append(asyncio.create_task(wrap_coroutine(file.get_async())))
+            pending_tasks.append(
+                asyncio.create_task(
+                    wrap_coroutine(file.get_async(include_activity=True))
+                )
+            )
         return pending_tasks
 
     def _resolve_sync_from_synapse_result(
         self,
         result: Union[None, "Folder", "File", BaseException],
         failure_strategy: FailureStrategy,
         synapse_client: Union[None, Synapse],
```

### Comparing `synapseclient-4.2.0/synapseclient/models/project.py` & `synapseclient-4.3.0/synapseclient/models/project.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/models/protocols/access_control_protocol.py` & `synapseclient-4.3.0/synapseclient/models/protocols/access_control_protocol.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/models/protocols/activity_protocol.py` & `synapseclient-4.3.0/synapseclient/models/protocols/activity_protocol.py`

 * *Files 24% similar despite different names*

```diff
@@ -84,7 +84,28 @@
             synapse_client: If not passed in or None this will use the last client
                 from the `.login()` method.
 
         Raises:
             ValueError: If the parent does not have an ID.
         """
         return None
+
+    @classmethod
+    async def disassociate_from_entity(
+        cls,
+        parent: Union["Table", "File"],
+        synapse_client: Optional[Synapse] = None,
+    ) -> None:
+        """
+        Disassociate the Activity from the parent entity. This is the first step in
+        deleting the Activity. If you have other entities that are associated with this
+        Activity you must disassociate them by calling this method on them as well.
+
+        Arguments:
+            parent: The parent entity this activity is associated with.
+            synapse_client: If not passed in or None this will use the last client
+                from the `.login()` method.
+
+        Raises:
+            ValueError: If the parent does not have an ID.
+        """
+        return None
```

### Comparing `synapseclient-4.2.0/synapseclient/models/protocols/annotations_protocol.py` & `synapseclient-4.3.0/synapseclient/models/protocols/annotations_protocol.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/models/protocols/file_protocol.py` & `synapseclient-4.3.0/synapseclient/models/protocols/file_protocol.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/models/protocols/folder_protocol.py` & `synapseclient-4.3.0/synapseclient/models/protocols/folder_protocol.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/models/protocols/project_protocol.py` & `synapseclient-4.3.0/synapseclient/models/protocols/project_protocol.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/models/protocols/storable_container_protocol.py` & `synapseclient-4.3.0/synapseclient/models/protocols/storable_container_protocol.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/models/protocols/table_protocol.py` & `synapseclient-4.3.0/synapseclient/models/protocols/table_protocol.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/models/protocols/team_protocol.py` & `synapseclient-4.3.0/synapseclient/models/protocols/team_protocol.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/models/protocols/user_protocol.py` & `synapseclient-4.3.0/synapseclient/models/protocols/user_protocol.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/models/services/search.py` & `synapseclient-4.3.0/synapseclient/models/services/search.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/models/services/storable_entity.py` & `synapseclient-4.3.0/synapseclient/models/services/storable_entity.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/models/services/storable_entity_components.py` & `synapseclient-4.3.0/synapseclient/models/services/storable_entity_components.py`

 * *Files 14% similar despite different names*

```diff
@@ -150,14 +150,57 @@
                 exception
             )
             if failure_strategy == FailureStrategy.RAISE_EXCEPTION:
                 raise exception
     return re_read_required
 
 
+def _has_activity_change_to_apply(
+    root_resource: Union["File", "Folder", "Project", "Table"],
+    last_persistent_instance: Union["File", "Folder", "Project", "Table"],
+) -> bool:
+    """Determines if there is a change on the Activity to apply to the root_resource.
+
+    Arguments:
+        root_resource: The root resource.
+        last_persistent_instance: The last persistent instance of the root resource.
+
+    Returns:
+        If the activity should be pulled forward.
+    """
+    return last_persistent_instance is None or (
+        (last_persistent_instance.activity != root_resource.activity)
+        or _pull_activity_forward_to_new_version(
+            root_resource=root_resource,
+            last_persistent_instance=last_persistent_instance,
+        )
+    )
+
+
+def _pull_activity_forward_to_new_version(
+    root_resource: Union["File", "Folder", "Project", "Table"],
+    last_persistent_instance: Union["File", "Folder", "Project", "Table"],
+) -> bool:
+    """Determine if there was a version update on the root_resource, and if so it
+    determines if we should be pulling the activity forward onto a new version.
+
+    Arguments:
+        root_resource: The root resource.
+        last_persistent_instance: The last persistent instance of the root resource.
+
+    Returns:
+        If the activity should be pulled forward.
+    """
+    return (
+        hasattr(root_resource, "associate_activity_to_new_version")
+        and root_resource.associate_activity_to_new_version
+        and last_persistent_instance.version_number != root_resource.version_number
+    )
+
+
 async def _store_activity_and_annotations(
     root_resource: Union["File", "Folder", "Project", "Table"],
     synapse_client: Optional[Synapse] = None,
 ) -> bool:
     """
     Function to store ancillary activity and annotations of an entity to synapse.
     This function is split off from the main store_entity_components function because
@@ -200,19 +243,19 @@
 
         root_resource.annotations = result.annotations
         root_resource.etag = result.etag
 
     if (
         hasattr(root_resource, "activity")
         and root_resource.activity is not None
-        and (
-            last_persistent_instance is None
-            or last_persistent_instance.activity != root_resource.activity
+        and _has_activity_change_to_apply(
+            root_resource=root_resource,
+            last_persistent_instance=last_persistent_instance,
         )
     ):
         result = await root_resource.activity.store_async(
             parent=root_resource, synapse_client=synapse_client
         )
-
         root_resource.activity = result
+
         return True
     return False
```

### Comparing `synapseclient-4.2.0/synapseclient/models/table.py` & `synapseclient-4.3.0/synapseclient/models/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -370,14 +370,20 @@
         version_number: The version number issued to this version on the object.
         version_label: The version label for this table
         version_comment: The version comment for this table
         is_latest_version: If this is the latest version of the object.
         is_search_enabled: When creating or updating a table or view specifies if full
             text search should be enabled. Note that enabling full text search might
             slow down the indexing of the table or view.
+        activity: The Activity model represents the main record of Provenance in
+            Synapse. It is analygous to the Activity defined in the
+            [W3C Specification](https://www.w3.org/TR/prov-n/) on Provenance. Activity
+            cannot be removed during a store operation by setting it to None. You must
+            use: [synapseclient.models.Activity.delete_async][] or
+            [synapseclient.models.Activity.disassociate_from_entity_async][].
         annotations: Additional metadata associated with the table. The key is the name
             of your desired annotations. The value is an object containing a list of
             values (use empty list to represent no values for key) and the value type
             associated with all values in the list. To remove all annotations set this
             to an empty dict `{}` or None and store the entity.
 
     """
@@ -435,15 +441,19 @@
     """When creating or updating a table or view specifies if full text search
     should be enabled. Note that enabling full text search might slow down the
     indexing of the table or view."""
 
     activity: Optional[Activity] = None
     """The Activity model represents the main record of Provenance in Synapse.  It is
     analygous to the Activity defined in the
-    [W3C Specification](https://www.w3.org/TR/prov-n/) on Provenance. """
+    [W3C Specification](https://www.w3.org/TR/prov-n/) on Provenance. Activity cannot
+    be removed during a store operation by setting it to None. You must use:
+    [synapseclient.models.Activity.delete_async][] or
+    [synapseclient.models.Activity.disassociate_from_entity_async][].
+    """
 
     annotations: Optional[
         Dict[
             str,
             Union[
                 List[str],
                 List[bool],
```

### Comparing `synapseclient-4.2.0/synapseclient/models/team.py` & `synapseclient-4.3.0/synapseclient/models/team.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/models/user.py` & `synapseclient-4.3.0/synapseclient/models/user.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/services/json_schema.py` & `synapseclient-4.3.0/synapseclient/services/json_schema.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/table.py` & `synapseclient-4.3.0/synapseclient/table.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/team.py` & `synapseclient-4.3.0/synapseclient/team.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient/wiki.py` & `synapseclient-4.3.0/synapseclient/wiki.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient.egg-info/PKG-INFO` & `synapseclient-4.3.0/synapseclient.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synapseclient
-Version: 4.2.0
+Version: 4.3.0
 Summary: A client for Synapse, a collaborative, open-source research platform that allows teams to share data, track analyses, and collaborate.
 Home-page: https://www.synapse.org
 Author: The Synapse Engineering Team
 Author-email: platform@sagebase.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/Sage-Bionetworks/synapsePythonClient
 Project-URL: Tracker, https://github.com/Sage-Bionetworks/synapsePythonClient/issues
@@ -39,35 +39,37 @@
 Requires-Dist: asyncio-atexit~=1.0.1
 Requires-Dist: httpx~=0.27.0
 Requires-Dist: tqdm<5.0,>=4.66.2
 Requires-Dist: loky~=3.0.0
 Requires-Dist: async-lru~=2.0.4
 Requires-Dist: psutil~=5.9.8
 Provides-Extra: dev
-Requires-Dist: pytest<7.0,>=6.0.0; extra == "dev"
+Requires-Dist: pytest<8.0,>=7.0.0; extra == "dev"
 Requires-Dist: pytest-mock<4.0,>=3.0; extra == "dev"
 Requires-Dist: pytest-socket~=0.6.0; extra == "dev"
-Requires-Dist: pytest-asyncio~=0.19; extra == "dev"
+Requires-Dist: pytest-asyncio<1.0,>=0.23.6; extra == "dev"
 Requires-Dist: flake8<4.0,>=3.7.0; extra == "dev"
 Requires-Dist: pytest-xdist[psutil]<3.0.0,>=2.2; extra == "dev"
 Requires-Dist: pytest-rerunfailures~=12.0; extra == "dev"
 Requires-Dist: func-timeout~=4.3; extra == "dev"
 Requires-Dist: pytest-cov~=4.1.0; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pandas<3.0,>=1.5; extra == "dev"
 Provides-Extra: tests
-Requires-Dist: pytest<7.0,>=6.0.0; extra == "tests"
+Requires-Dist: pytest<8.0,>=7.0.0; extra == "tests"
 Requires-Dist: pytest-mock<4.0,>=3.0; extra == "tests"
 Requires-Dist: pytest-socket~=0.6.0; extra == "tests"
-Requires-Dist: pytest-asyncio~=0.19; extra == "tests"
+Requires-Dist: pytest-asyncio<1.0,>=0.23.6; extra == "tests"
 Requires-Dist: flake8<4.0,>=3.7.0; extra == "tests"
 Requires-Dist: pytest-xdist[psutil]<3.0.0,>=2.2; extra == "tests"
 Requires-Dist: pytest-rerunfailures~=12.0; extra == "tests"
 Requires-Dist: func-timeout~=4.3; extra == "tests"
 Requires-Dist: pytest-cov~=4.1.0; extra == "tests"
+Requires-Dist: pandas<3.0,>=1.5; extra == "tests"
 Provides-Extra: pandas
 Requires-Dist: pandas<3.0,>=1.5; extra == "pandas"
 Provides-Extra: pysftp
 Requires-Dist: pysftp<0.3,>=0.2.8; extra == "pysftp"
 Provides-Extra: boto3
 Requires-Dist: boto3<2.0,>=1.7.0; extra == "boto3"
 Provides-Extra: docs
@@ -121,33 +123,48 @@
 
 **Starting from Synapse Python client version 3.0, Synapse Python client requires Python >= 3.8**
 
 ### Install using pip
 
 The [Python Synapse Client is on PyPI](https://pypi.python.org/pypi/synapseclient) and can be installed with pip:
 
-    (sudo) pip install synapseclient[pandas,pysftp]
+    # Here are a few ways to install the client. Choose the one that fits your use-case
+    # sudo may optionally be needed depending on your setup
+
+    pip install --upgrade synapseclient
+    pip install --upgrade "synapseclient[pandas]"
+    pip install --upgrade "synapseclient[pandas, pysftp, boto3]"
 
 ...or to upgrade an existing installation of the Synapse client:
 
-    (sudo) pip install --upgrade synapseclient
+    # sudo may optionally be needed depending on your setup
+    pip install --upgrade synapseclient
 
-The dependencies on `pandas` and `pysftp` are optional. Synapse [Tables](https://python-docs.synapse.org/reference/tables/) integrate
+The dependencies on `pandas`, `pysftp`, and `boto3` are optional. Synapse
+[Tables](https://python-docs.synapse.org/reference/tables/) integrate
 with [Pandas](http://pandas.pydata.org/). The library `pysftp` is required for users of
-[SFTP](https://python-docs.synapse.org/guides/data_storage/#sftp) file storage. Both libraries require native code
-to be compiled or installed separately from prebuilt binaries.
+[SFTP](https://python-docs.synapse.org/guides/data_storage/#sftp) file storage. All
+libraries require native code to be compiled or installed separately from prebuilt
+binaries.
 
 ### Install from source
 
 Clone the [source code repository](https://github.com/Sage-Bionetworks/synapsePythonClient).
 
     git clone git://github.com/Sage-Bionetworks/synapsePythonClient.git
     cd synapsePythonClient
     pip install .
 
+Alternatively, you can use pip to install a particular branch, commit, or other git reference:
+
+    pip install git+https://github.com/Sage-Bionetworks/synapsePythonClient@master
+
+or
+
+    pip install git+https://github.com/Sage-Bionetworks/synapsePythonClient@my-commit-hash
 
 Command line usage
 ------------------
 
 The Synapse client can be used from the shell command prompt. Valid commands
 include: query, get, cat, add, update, delete, and onweb. A few examples are
 shown.
```

### Comparing `synapseclient-4.2.0/synapseclient.egg-info/SOURCES.txt` & `synapseclient-4.3.0/synapseclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseclient.egg-info/requires.txt` & `synapseclient-4.3.0/synapseclient.egg-info/requires.txt`

 * *Files 13% similar despite different names*

```diff
@@ -12,25 +12,26 @@
 async-lru~=2.0.4
 psutil~=5.9.8
 
 [boto3]
 boto3<2.0,>=1.7.0
 
 [dev]
-pytest<7.0,>=6.0.0
+pytest<8.0,>=7.0.0
 pytest-mock<4.0,>=3.0
 pytest-socket~=0.6.0
-pytest-asyncio~=0.19
+pytest-asyncio<1.0,>=0.23.6
 flake8<4.0,>=3.7.0
 pytest-xdist[psutil]<3.0.0,>=2.2
 pytest-rerunfailures~=12.0
 func-timeout~=4.3
 pytest-cov~=4.1.0
 black
 pre-commit
+pandas<3.0,>=1.5
 
 [docs]
 mkdocs>=1.5.3
 mkdocs-material>=9.4.14
 mkdocstrings>=0.24.0
 mkdocstrings-python>=1.7.5
 termynal>=0.11.1
@@ -40,16 +41,17 @@
 [pandas]
 pandas<3.0,>=1.5
 
 [pysftp]
 pysftp<0.3,>=0.2.8
 
 [tests]
-pytest<7.0,>=6.0.0
+pytest<8.0,>=7.0.0
 pytest-mock<4.0,>=3.0
 pytest-socket~=0.6.0
-pytest-asyncio~=0.19
+pytest-asyncio<1.0,>=0.23.6
 flake8<4.0,>=3.7.0
 pytest-xdist[psutil]<3.0.0,>=2.2
 pytest-rerunfailures~=12.0
 func-timeout~=4.3
 pytest-cov~=4.1.0
+pandas<3.0,>=1.5
```

### Comparing `synapseclient-4.2.0/synapseutils/__init__.py` & `synapseclient-4.3.0/synapseutils/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 ## Overview
 
 The ``synapseutils`` package provides both higher level beta functions as well as utilities for interacting with
 [Synapse](http://www.synapse.org).  The behavior of these functions are subject to change.
 
 """
+
 # flake8: noqa F401 unclear who is using these
 from .copy_functions import copy, copyWiki, copyFileHandles, changeFileMetaData
 from .walk_functions import walk
 from .sync import syncFromSynapse, syncToSynapse, generate_sync_manifest
 from .migrate_functions import index_files_for_migration, migrate_indexed_files
-from .monitor import notifyMe, with_progress_bar
+from .monitor import notifyMe, with_progress_bar, notify_me_async
 from .describe_functions import describe
```

### Comparing `synapseclient-4.2.0/synapseutils/copy_functions.py` & `synapseclient-4.3.0/synapseutils/copy_functions.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseutils/describe_functions.py` & `synapseclient-4.3.0/synapseutils/describe_functions.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseutils/migrate_functions.py` & `synapseclient-4.3.0/synapseutils/migrate_functions.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.2.0/synapseutils/sync.py` & `synapseclient-4.3.0/synapseutils/sync.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,48 +1,55 @@
+"""This module is responsible for holding sync to/from synapse utility functions."""
 import ast
-import csv
+import asyncio
 import concurrent.futures
-from contextlib import contextmanager
+import csv
 import datetime
 import io
 import os
 import re
 import sys
 import threading
-import typing
+from contextlib import contextmanager
+from dataclasses import dataclass
+from typing import Dict, Iterable, List, NamedTuple, Union
 
-from .monitor import notifyMe
-from synapseclient.entity import is_container
-from synapseclient.core import config
-from synapseclient.core.utils import (
-    id_of,
-    is_url,
-    is_synapse_id_str,
-    datetime_or_none,
-    bool_or_none,
-)
-from synapseclient import File, table, Synapse
-from synapseclient.core.pool_provider import SingleThreadExecutor
-from synapseclient.core import utils
+from tqdm import tqdm
+
+from synapseclient import File as SynapseFile
+from synapseclient import Synapse, table
+from synapseclient.core import config, utils
+from synapseclient.core.async_utils import wrap_async_to_sync
 from synapseclient.core.cumulative_transfer_progress import CumulativeTransferProgress
 from synapseclient.core.exceptions import (
+    SynapseError,
     SynapseFileNotFoundError,
     SynapseHTTPError,
     SynapseProvenanceError,
 )
 from synapseclient.core.multithread_download.download_threads import (
     shared_executor as download_shared_executor,
 )
-from synapseclient.core.upload.multipart_upload import (
-    shared_executor as upload_shared_executor,
+from synapseclient.core.pool_provider import SingleThreadExecutor
+from synapseclient.core.upload.multipart_upload_async import shared_progress_bar
+from synapseclient.core.utils import (
+    bool_or_none,
+    datetime_or_none,
+    get_synid_and_version,
+    id_of,
+    is_synapse_id_str,
+    is_url,
 )
-from opentelemetry import context, trace
-from opentelemetry.context import Context
+from synapseclient.entity import is_container
+from synapseclient.models import Activity, File, UsedEntity, UsedURL
 
+from .monitor import notify_me_async
 
+# When new fields are added to the manifest they will also need to be added to
+# file.py#_determine_fields_to_ignore_in_merge
 REQUIRED_FIELDS = ["path", "parent"]
 FILE_CONSTRUCTOR_FIELDS = ["name", "id", "synapseStore", "contentType"]
 STORE_FUNCTION_FIELDS = ["activityName", "activityDescription", "forceVersion"]
 PROVENANCE_FIELDS = ["used", "executed"]
 MAX_RETRIES = 4
 MANIFEST_FILENAME = "SYNAPSE_METADATA_MANIFEST.tsv"
 DEFAULT_GENERATED_MANIFEST_KEYS = [
@@ -328,15 +335,15 @@
                 entity, path, ifcollision, followLink, progress, downloadFile, manifest
             )
 
             # once the whole folder hierarchy has been traversed this entrant thread
             # waits for all file downloads to complete before returning
             files = root_folder_sync.wait_until_finished()
 
-        elif isinstance(entity, File):
+        elif isinstance(entity, SynapseFile):
             files = [entity]
 
         else:
             raise ValueError(
                 "Cannot initiate a sync from an entity that is not a File or Folder"
             )
 
@@ -371,15 +378,15 @@
                     ifcollision=ifcollision,
                     followLink=followLink,
                     downloadFile=downloadFile,
                 )
 
             files = []
             provenance = None
-            if isinstance(entity, File):
+            if isinstance(entity, SynapseFile):
                 if path:
                     entity_provenance = _get_file_entity_provenance_dict(
                         self._syn, entity
                     )
                     provenance = {entity_id: entity_provenance}
 
                 files.append(entity)
@@ -496,285 +503,256 @@
                     folder_stack.append(
                         (child_folder, folder_path, folder_sync, create_child_manifest)
                     )
 
         return root_folder_sync
 
 
-class _PendingProvenance:
-    def __init__(self):
-        self._pending = set()
-        self._pending_count = 0
-
-    def update(self, pending: set):
-        """Add pending items"""
-        self._pending_count += len(pending.difference(self._pending))
-        self._pending.update(pending)
-
-    def finished(self, provenance):
-        """Remove the given provenance after it is finished uploading"""
-        self._pending.remove(provenance)
-
-    def has_pending(self):
-        """Return whether any pending provenance was recorded"""
-        return self._pending_count > 0
-
-    def has_finished_provenance(self):
-        """Return whether any of the pending provenance has finished"""
-        return len(self._pending) < self._pending_count
-
-    def reset_count(self):
-        """Reset the pending count to reflect the current pending state"""
-        self._pending_count = len(self._pending)
-
+class _SyncUploadItem(NamedTuple):
+    """Represents a single file being uploaded.
 
-class _SyncUploadItem(typing.NamedTuple):
-    """Represents a single file being uploaded"""
+    Attributes:
+        entity: The file that is going through the sync process.
+        used: Concept from Activity that can be a URL, Synapse ID, or path to a file.
+        executed: Concept from Activity that can be a URL, Synapse ID, or path to a
+            file.
+        activity_name: The name of the activity that is being performed.
+        activity_description: The description of the activity that is being performed.
+    """
 
     entity: File
-    used: typing.Iterable[str]
-    executed: typing.Iterable[str]
-    store_kwargs: typing.Mapping
+    used: Iterable[str]
+    executed: Iterable[str]
+    activity_name: str
+    activity_description: str
 
 
+@dataclass
 class _SyncUploader:
     """
     Manages the uploads associated associated with a syncToSynapse call.
     Files will be uploaded concurrently and in an order that honors any
     interdependent provenance.
 
     """
 
-    def __init__(
-        self,
-        syn: Synapse,
-        executor: concurrent.futures.Executor,
-        max_concurrent_file_transfers: int = None,
-    ):
+    syn: Synapse
+
+    @dataclass
+    class DependencyGraph:
+        """The graph that represents the dependencies of the files to be uploaded.
+
+        Attributes:
+            path_to_dependencies: A dictionary where the key is the path of the file and
+                the value is a list of paths that need to be uploaded before the key can
+                be uploaded.
+            path_to_upload_item: A dictionary where the key is the path of the file and
+                the value is the upload item that is associated with the file.
+            path_to_file_check: A dictionary where the key is the path of the file and
+                the value is a boolean that represents if the file is a file or not.
         """
-        Arguments:
-            syn: A synapse client
-            executor: An ExecutorService in which concurrent file downloads
-                      can be scheduled
+
+        path_to_dependencies: Dict[str, List[str]]
+        path_to_upload_item: Dict[str, _SyncUploadItem]
+        path_to_file_check: Dict[str, bool]
+
+    def _build_dependency_graph(
+        self, items: Iterable[_SyncUploadItem]
+    ) -> DependencyGraph:
         """
-        self._syn = syn
+        Determine the order in which the files should be uploaded based on their
+        dependencies. This will also verify that the dependencies are valid and that
+        there are no cycles in the graph.
 
-        max_concurrent_file_transfers = max(
-            int(max_concurrent_file_transfers or self._syn.max_threads / 2), 1
-        )
-        self._executor = executor
-        self._file_semaphore = threading.BoundedSemaphore(max_concurrent_file_transfers)
+        Arguments:
+            items: The list of items to upload.
 
-    @staticmethod
-    def _order_items(items):
-        # order items by their interdependent provenance and raise any dependency
-        # errors
+        Return:
+            A graph that represents information about how to upload the graph of items
+            into Synapse.
+        """
 
         items_by_path = {i.entity.path: i for i in items}
         graph = {}
+        resolved_file_checks = {}
 
         for item in items:
             item_file_provenance = []
             for provenance_dependency in item.used + item.executed:
-                if os.path.isfile(provenance_dependency):
+                is_file = resolved_file_checks.get(
+                    provenance_dependency, None
+                ) or os.path.isfile(provenance_dependency)
+                if provenance_dependency not in resolved_file_checks:
+                    resolved_file_checks.update({provenance_dependency: is_file})
+                if is_file:
                     if provenance_dependency not in items_by_path:
                         # an upload lists provenance of a file that is not itself
                         # included in the upload
                         raise ValueError(
                             f"{item.entity.path} depends on"
                             f" {provenance_dependency} which is not being uploaded"
                         )
 
                     item_file_provenance.append(provenance_dependency)
 
             graph[item.entity.path] = item_file_provenance
 
+        # Used to verify that the graph does not contain any cycles
         graph_sorted = utils.topolgical_sort(graph)
-        return [items_by_path[i[0]] for i in graph_sorted]
+        path_to_dependencies_sorted = {}
+        path_to_upload_items_sorted = {}
+        for path, dependency_paths in graph_sorted:
+            path_to_dependencies_sorted.update({path: dependency_paths})
+            path_to_upload_items_sorted.update({path: items_by_path.get(path)})
+
+        return self.DependencyGraph(
+            path_to_dependencies=path_to_dependencies_sorted,
+            path_to_upload_item=path_to_upload_items_sorted,
+            path_to_file_check=resolved_file_checks,
+        )
 
-    @staticmethod
-    def _convert_provenance(provenance, finished_items):
-        # convert any string file path provenance to the corresponding entity that
-        # has been uploaded
-
-        converted_provenance = []
-        pending_provenance = set()
-        for p in provenance:
-            if os.path.isfile(p):
-                converted = finished_items.get(p)
-                if converted:
-                    converted_provenance.append(converted)
-                else:
-                    pending_provenance.add(p)
-            else:
-                converted_provenance.append(p)
+    def _build_tasks_from_dependency_graph(
+        self, dependency_graph: DependencyGraph
+    ) -> List[asyncio.Task]:
+        """
+        Build the asyncio tasks that will be used to upload the files in the correct
+        order based on their dependencies.
 
-        return converted_provenance, pending_provenance
+        Arguments:
+            dependency_graph: The graph that represents the dependencies of the files to
+                be uploaded.
 
-    @staticmethod
-    def _abort(futures):
-        # abort this sync because of an error
-
-        exception = None
-        for future in futures:
-            if future.done():
-                exception = exception or future.exception()
-            else:
-                future.cancel()
+        Return:
+            A list of asyncio tasks that will upload the files in the correct order.
 
-        # if we are aborted by definition one of the futures should have an
-        # exception.
-        # if somehow not from None fuctions fine
-        raise ValueError("Sync aborted due to upload failure") from exception
-
-    def upload(self, items: typing.Iterable[_SyncUploadItem]):
-        progress = CumulativeTransferProgress("Uploaded")
-
-        # flag to set in a child in an upload thread if an error occurs to signal
-        # to the entrant thread to stop processing.
-        abort_event = threading.Event()
-
-        # used to lock around shared state and to notify when dependencies are
-        # resolved so that provenance dependent files can be uploaded
-        dependency_condition = threading.Condition()
-
-        pending_provenance = _PendingProvenance()
-        finished_items = {}
-
-        ordered_items = self._order_items([i for i in items])
-
-        futures = []
-        while ordered_items:
-            skipped_items = []
-            for item in ordered_items:
-                if abort_event.is_set():
-                    # if this flag is set, one of the upload threads failed and we
-                    # should raise it's error and cancel any remaining futures
-                    self._abort(futures)
-
-                with dependency_condition:
-                    used, used_pending = self._convert_provenance(
-                        item.used, finished_items
-                    )
-                    executed, executed_pending = self._convert_provenance(
-                        item.executed, finished_items
-                    )
+        """
+        created_tasks_by_path = {}
 
-                    if used_pending or executed_pending:
-                        # we can't upload this item yet, it has provenance that
-                        # hasn't yet been uploaded
-                        skipped_items.append(item)
-                        pending_provenance.update(used_pending.union(executed_pending))
-
-                        # skip uploading because dependent provenance hasn't
-                        # finished uploading
-                        continue
-
-                # else not continued above due to pending provenance
-                # all provenance that this item depends on has already been uploaded
-                # so we can go ahead and upload this item
-
-                # we acquire the semaphore to ensure that we aren't uploading more
-                # than our configured maximum number of files here at once. once we
-                # reach the limit we'll block here until one of the existing file uploads completes
-                self._file_semaphore.acquire()
-                trace.get_current_span().set_attributes(
-                    {"thread.id": threading.get_ident()}
-                )
-                future = self._executor.submit(
-                    self._upload_item,
-                    item,
-                    used,
-                    executed,
-                    finished_items,
-                    pending_provenance,
-                    dependency_condition,
-                    abort_event,
-                    progress,
-                    context.get_current(),
+        # Because the graph is sorted in topological order, we can iterate over the
+        # paths in order and create a task for each file. This ensures that before we
+        # get to any files that have a dependency the Task to save the dependency has
+        # already been created.
+        for (
+            file_path,
+            dependent_file_paths,
+        ) in dependency_graph.path_to_dependencies.items():
+            dependent_tasks = []
+            for dependent_file in dependent_file_paths:
+                if dependency_graph.path_to_file_check.get(dependent_file, None):
+                    dependent_tasks.append(created_tasks_by_path.get(dependent_file))
+
+            upload_item = dependency_graph.path_to_upload_item.get(file_path)
+            file_task = asyncio.create_task(
+                coro=self._upload_item_async(
+                    item=upload_item.entity,
+                    used=upload_item.used,
+                    executed=upload_item.executed,
+                    activity_name=upload_item.activity_name,
+                    activity_description=upload_item.activity_description,
+                    dependent_futures=dependent_tasks,
                 )
-                futures.append(future)
+            )
+            created_tasks_by_path.update({file_path: file_task})
 
-            with dependency_condition:
-                if pending_provenance.has_pending():
-                    # skipped_items contains all the items that we couldn't upload
-                    # the previous time through the loop because they depended on
-                    # another item for provenance. wait until there at least one
-                    # those items finishes before continuing another time through the loop.
-                    if not abort_event.is_set():
-                        dependency_condition.wait_for(
-                            lambda: (
-                                pending_provenance.has_finished_provenance()
-                                or abort_event.is_set()
-                            )
-                        )
+        return created_tasks_by_path.values()
+
+    async def upload(self, items: Iterable[_SyncUploadItem]) -> None:
+        """Upload a number of files to Synapse as provided in the manifest file. This
+        will handle ordering the files based on their dependency graph.
 
-                pending_provenance.reset_count()
+        Arguments:
+            items: The list of items to upload.
+
+        Returns:
+            None
+        """
+        dependency_graph = self._build_dependency_graph(items=[i for i in items])
+        tasks = self._build_tasks_from_dependency_graph(
+            dependency_graph=dependency_graph
+        )
 
-            ordered_items = skipped_items
+        await asyncio.gather(*tasks)
 
-        # all items have been submitted for upload
+    def _build_activity_linkage(
+        self, used_or_executed: Iterable[str], resolved_file_ids: Dict[str, str]
+    ) -> List[Union[UsedEntity, UsedURL]]:
+        """Loop over the incoming list of used or executed items and build the
+        appropriate UsedEntity or UsedURL objects.
 
-        concurrent.futures.wait(futures, return_when=concurrent.futures.FIRST_EXCEPTION)
-        if abort_event.is_set():
-            # at least one item failed to upload
-            self._abort(futures)
+        Arguments:
+            used_or_executed: The list of used or executed items.
+            resolved_file_ids: A dictionary that maps the path of a file to its Synapse
+                ID.
 
-    def _upload_item(
+        Returns:
+            A list of UsedEntity or UsedURL objects.
+        """
+        returned_linkage = []
+        for item in used_or_executed:
+            resolved_file_id = resolved_file_ids.get(item, None)
+            if resolved_file_id:
+                returned_linkage.append(UsedEntity(target_id=resolved_file_id))
+            elif is_url(item):
+                returned_linkage.append(UsedURL(url=item))
+
+            # -- Synapse Entity ID (assuming the string is an ID)
+            elif isinstance(item, str):
+                if not is_synapse_id_str(item):
+                    raise ValueError(f"{item} is not a valid Synapse id")
+                synid, version = get_synid_and_version(
+                    item
+                )  # Handle synapseIds of from syn234.4
+                target_version = None
+                if version:
+                    target_version = int(version)
+                returned_linkage.append(
+                    UsedEntity(target_id=synid, target_version_number=target_version)
+                )
+            else:
+                raise SynapseError(
+                    f"Unexpected parameters in used or executed Activity fields: {item}."
+                )
+        return returned_linkage
+
+    async def _upload_item_async(
         self,
-        item,
-        used,
-        executed,
-        finished_items,
-        pending_provenance,
-        dependency_condition,
-        abort_event,
-        progress,
-        otel_context: typing.Union[Context, None],
-    ):
-        if otel_context:
-            context.attach(otel_context)
-        try:
-            with upload_shared_executor(self._executor):
-                # we configure an upload thread local shared executor so that any
-                # multipart uploads that result from this upload will share the
-                # executor of this sync rather than creating their own threadpool.
-
-                with progress.accumulate_progress():
-                    entity = self._syn.store(
-                        item.entity,
-                        used=used,
-                        executed=executed,
-                        **item.store_kwargs,
-                        async_file_handle_upload=False,
-                    )
+        item: File,
+        used: Iterable[str],
+        executed: Iterable[str],
+        activity_name: str,
+        activity_description: str,
+        dependent_futures: List[asyncio.Future],
+    ) -> File:
+        resolved_file_ids = {}
+        if dependent_futures:
+            finished_dependencies, pending = await asyncio.wait(dependent_futures)
+            if pending:
+                raise RuntimeError(
+                    f"There were {len(pending)} dependencies left when storing {item}"
+                )
+            for finished_dependency in finished_dependencies:
+                result = finished_dependency.result()
+                resolved_file_ids.update({result.path: result.id})
 
-                with dependency_condition:
-                    finished_items[item.entity.path] = entity
-                    try:
-                        pending_provenance.finished(item.entity.path)
-
-                        # this item was defined as provenance for another item, now
-                        # that it's finished we may be able to upload that depending
-                        # item, so wake up he central thread
-                        dependency_condition.notify_all()
-
-                    except KeyError:
-                        # this item is not used in provenance of another item,
-                        # that's fine
-                        pass
-
-        except Exception:
-            with dependency_condition:
-                abort_event.set()
-                dependency_condition.notify_all()
-            raise
+        used_activity = self._build_activity_linkage(
+            used_or_executed=used, resolved_file_ids=resolved_file_ids
+        )
+        executed_activity = self._build_activity_linkage(
+            used_or_executed=executed, resolved_file_ids=resolved_file_ids
+        )
 
-        finally:
-            self._file_semaphore.release()
+        if used_activity or executed_activity:
+            item.activity = Activity(
+                name=activity_name,
+                description=activity_description,
+                used=used_activity,
+                executed=executed_activity,
+            )
+        await item.store_async()
+        return item
 
 
 def generateManifest(syn, allFiles, filename, provenance_cache=None) -> None:
     """Generates a manifest file based on a list of entities objects.
 
     [Read more about the manifest file format](../../explanations/manifest_tsv/)
 
@@ -869,15 +847,15 @@
         if e.response.status_code == 404:
             return {}  # No provenance present return empty dict
         else:
             raise  # unexpected error so we re-raise the exception
 
 
 def _convert_manifest_data_items_to_string_list(
-    items: typing.List[typing.Union[str, datetime.datetime, bool, int, float]],
+    items: List[Union[str, datetime.datetime, bool, int, float]],
 ) -> str:
     """
     Handle coverting an individual key that contains a possible list of data into a
     list of strings or objects that can be written to the manifest file.
 
     This has specific logic around how to handle datetime fields.
 
@@ -939,15 +917,15 @@
 
     if len(items) > 1:
         return f'[{",".join(items_to_write)}]'
     else:
         return items_to_write[0]
 
 
-def _convert_manifest_data_row_to_dict(row: dict, keys: typing.List[str]) -> dict:
+def _convert_manifest_data_row_to_dict(row: dict, keys: List[str]) -> dict:
     """
     Convert a row of data to a dict that can be written to a manifest file.
 
     Args:
         row: The row of data to convert.
         keys: The keys of the manifest. Used to select the rows of data.
 
@@ -961,17 +939,15 @@
             items_to_write = _convert_manifest_data_items_to_string_list(data_for_key)
             data_to_write[key] = items_to_write
         else:
             data_to_write[key] = data_for_key
     return data_to_write
 
 
-def _write_manifest_data(
-    filename: str, keys: typing.List[str], data: typing.List[dict]
-) -> None:
+def _write_manifest_data(filename: str, keys: List[str], data: List[dict]) -> None:
     """
     Write a number of keys and a list of data to a manifest file. This will write
     the data out as a tab separated file.
 
     For the data we are writing to the TSV file we are not quoting the content with any
     characters. This is because the syncToSynapse function does not require strings to
     be quoted. When quote characters were included extra double quotes were being added
@@ -1161,15 +1137,21 @@
             )
             raise SynapseHTTPError
     sys.stdout.write("OK\n")
     return df
 
 
 def syncToSynapse(
-    syn, manifestFile, dryRun=False, sendMessages=True, retries=MAX_RETRIES
+    syn: Synapse,
+    manifestFile,
+    dryRun: bool = False,
+    sendMessages: bool = True,
+    retries: int = MAX_RETRIES,
+    merge_existing_annotations: bool = True,
+    associate_activity_to_new_version: bool = False,
 ) -> None:
     """Synchronizes files specified in the manifest file to Synapse.
 
     Given a file describing all of the uploads, this uploads the content to Synapse and
     optionally notifies you via Synapse messagging (email) at specific intervals, on
     errors and on completion.
 
@@ -1193,46 +1175,81 @@
     since epoch.
 
     Arguments:
         syn: A Synapse object with user's login, e.g. syn = synapseclient.login()
         manifestFile: A tsv file with file locations and metadata to be pushed to Synapse.
         dryRun: Performs validation without uploading if set to True.
         sendMessages: Sends out messages on completion if set to True.
+        retries: Number of retries to attempt if an error occurs.
+        merge_existing_annotations: If True, will merge the annotations in the manifest
+            file with the existing annotations on Synapse. If False, will overwrite the
+            existing annotations on Synapse with the annotations in the manifest file.
+        associate_activity_to_new_version: If True, and a version update occurs, the
+            existing activity in Synapse will be associated with the new version. The
+            exception is if you are specifying new values to be used/executed, it will
+            create a new activity for the new version of the entity.
 
     Returns:
         None
     """
     df = readManifestFile(syn, manifestFile)
-    # have to check all size of single file
+
     sizes = [
         os.stat(os.path.expandvars(os.path.expanduser(f))).st_size
         for f in df.path
         if not is_url(f)
     ]
-    # Write output on what is getting pushed and estimated times - send out message.
-    sys.stdout.write("=" * 50 + "\n")
-    sys.stdout.write(
-        "We are about to upload %i files with a total size of %s.\n "
-        % (len(df), utils.humanizeBytes(sum(sizes)))
+
+    total_upload_size = sum(sizes)
+
+    syn.logger.info(
+        f"We are about to upload {len(df)} files with a total size of {total_upload_size}."
     )
-    sys.stdout.write("=" * 50 + "\n")
 
     if dryRun:
+        syn.logger.info("Returning due to Dry Run.")
         return
 
-    sys.stdout.write("Starting upload...\n")
-    if sendMessages:
-        notify_decorator = notifyMe(syn, "Upload of %s" % manifestFile, retries=retries)
-        upload = notify_decorator(_manifest_upload)
-        upload(syn, df)
-    else:
-        _manifest_upload(syn, df)
+    progress_bar = tqdm(
+        total=total_upload_size,
+        desc=f"Uploading {len(df)} files",
+        unit="B",
+        unit_scale=True,
+        smoothing=0,
+    )
+    with shared_progress_bar(progress_bar):
+        if sendMessages:
+            notify_decorator = notify_me_async(
+                syn, "Upload of %s" % manifestFile, retries=retries
+            )
+            upload = notify_decorator(_manifest_upload)
+            wrap_async_to_sync(
+                upload(
+                    syn,
+                    df,
+                    merge_existing_annotations,
+                    associate_activity_to_new_version,
+                ),
+                syn,
+            )
+        else:
+            wrap_async_to_sync(
+                _manifest_upload(
+                    syn,
+                    df,
+                    merge_existing_annotations,
+                    associate_activity_to_new_version,
+                ),
+                syn,
+            )
+        progress_bar.update(total_upload_size - progress_bar.n)
+        progress_bar.close()
 
 
-def _split_string(input_string: str) -> typing.List[str]:
+def _split_string(input_string: str) -> List[str]:
     """
     Use regex to split a string apart by commas that are not inside of double quotes.
 
 
     Args:
         input_string: A string to split apart.
 
@@ -1247,15 +1264,15 @@
         modified_row.append(modified_item)
 
     return modified_row
 
 
 def _convert_cell_in_manifest_to_python_types(
     cell: str,
-) -> typing.Union[typing.List, datetime.datetime, float, int, bool, str]:
+) -> Union[List, datetime.datetime, float, int, bool, str]:
     """
     Takes a possibly comma delimited cell from the manifest TSV file into a list
     of items to be used as annotations.
 
     Args:
         cell: The cell item to convert.
 
@@ -1290,69 +1307,118 @@
                 value_to_add = ast.literal_eval(node_or_string=annotation_value)
             except (ValueError, SyntaxError):
                 value_to_add = annotation_value
             values_to_return.append(value_to_add)
     return values_to_return[0] if len(values_to_return) == 1 else values_to_return
 
 
-def _manifest_upload(syn: Synapse, df) -> bool:
+def _build_annotations_for_file(
+    manifest_annotations,
+) -> Dict[
+    str,
+    Union[
+        List[str],
+        List[bool],
+        List[float],
+        List[int],
+        List[datetime.date],
+        List[datetime.datetime],
+    ],
+]:
+    """Pull the annotations out of the format defined in the manifest being uploaded
+    into a format that is expected internally within the client. For annotations
+    that might not contain a value we will assume it to be None and it won't be uploaded
+    as a blank annotation.
+
+
+    Arguments:
+        manifest_annotations: The annotations as defined in the manifest file.
+
+    Returns:
+        The annoations in a format used in the client.
+    """
+    # if a item in the manifest upload is an empty string we do not want to upload that
+    # as an empty string annotation
+    file_annotations = {}
+
+    for annotation_key, annotation_value in manifest_annotations.items():
+        if annotation_value is None or annotation_value == "":
+            continue
+        if isinstance(annotation_value, str):
+            file_annotations[
+                annotation_key
+            ] = _convert_cell_in_manifest_to_python_types(cell=annotation_value)
+        else:
+            file_annotations[annotation_key] = annotation_value
+    return file_annotations
+
+
+async def _manifest_upload(
+    syn: Synapse,
+    df,
+    merge_existing_annotations: bool = True,
+    associate_activity_to_new_version: bool = False,
+) -> bool:
     """
     Handles the upload of the manifest file.
 
     Args:
         syn: The logged in Synapse client.
         df: The dataframe of the manifest file.
+        merge_existing_annotations: If True, will merge the annotations in the manifest
+            file with the existing annotations on Synapse. If False, will overwrite the
+            existing annotations on Synapse with the annotations in the manifest file.
+        associate_activity_to_new_version: If True, and a version update occurs, the
+            existing activity in Synapse will be associated with the new version. The
+            exception is if you are specifying new values to be used/executed, it will
+            create a new activity for the new version of the entity.
 
     Returns:
         If the manifest upload was successful.
     """
     items = []
     for _, row in df.iterrows():
         file = File(
             path=row["path"],
-            parent=row["parent"],
-            **{key: row[key] for key in FILE_CONSTRUCTOR_FIELDS if key in row},
+            parent_id=row["parent"],
+            name=row["name"] if "name" in row else None,
+            id=row["id"] if "id" in row else None,
+            synapse_store=row["synapseStore"] if "synapseStore" in row else True,
+            content_type=row["contentType"] if "contentType" in row else None,
+            force_version=row["forceVersion"] if "forceVersion" in row else True,
+            merge_existing_annotations=merge_existing_annotations,
+            associate_activity_to_new_version=associate_activity_to_new_version,
+            _present_manifest_fields=row.keys().tolist(),
         )
 
-        annotations = dict(
+        manifest_style_annotations = dict(
             row.drop(
                 FILE_CONSTRUCTOR_FIELDS
                 + STORE_FUNCTION_FIELDS
                 + REQUIRED_FIELDS
                 + PROVENANCE_FIELDS,
                 errors="ignore",
             )
         )
 
-        # if a item in the manifest upload is an empty string we do not want to upload that
-        # as an empty string annotation
-        file_annotations = {}
-
-        for annotation_key, annotation_value in annotations.items():
-            if annotation_value is None or annotation_value == "":
-                continue
-            if isinstance(annotation_value, str):
-                file_annotations[
-                    annotation_key
-                ] = _convert_cell_in_manifest_to_python_types(cell=annotation_value)
-            else:
-                file_annotations[annotation_key] = annotation_value
-        file.annotations = file_annotations
+        file.annotations = _build_annotations_for_file(manifest_style_annotations)
 
         item = _SyncUploadItem(
             file,
             row["used"] if "used" in row else [],
             row["executed"] if "executed" in row else [],
-            {key: row[key] for key in STORE_FUNCTION_FIELDS if key in row},
+            activity_name=row["activityName"] if "activityName" in row else None,
+            activity_description=row["activityDescription"]
+            if "activityDescription" in row
+            else None,
         )
         items.append(item)
 
-    with _sync_executor(syn) as executor:
-        uploader = _SyncUploader(syn, executor)
-        uploader.upload(items)
+    uploader = _SyncUploader(syn)
+    await uploader.upload(items)
 
     return True
 
 
 def _check_file_name(df):
     compiled = re.compile(r"^[`\w \-\+\.\(\)]{1,256}$")
     for idx, row in df.iterrows():
```

### Comparing `synapseclient-4.2.0/synapseutils/walk_functions.py` & `synapseclient-4.3.0/synapseutils/walk_functions.py`

 * *Files identical despite different names*

