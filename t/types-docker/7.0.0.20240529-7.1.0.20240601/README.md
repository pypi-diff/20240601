# Comparing `tmp/types-docker-7.0.0.20240529.tar.gz` & `tmp/types-docker-7.1.0.20240601.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-docker-7.0.0.20240529.tar", last modified: Wed May 29 02:25:23 2024, max compression
+gzip compressed data, was "types-docker-7.1.0.20240601.tar", last modified: Sat Jun  1 02:27:29 2024, max compression
```

## Comparing `types-docker-7.0.0.20240529.tar` & `types-docker-7.1.0.20240601.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:25:23.671215 types-docker-7.0.0.20240529/
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-29 02:25:21.000000 types-docker-7.0.0.20240529/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-29 02:25:21.000000 types-docker-7.0.0.20240529/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-29 02:25:23.671215 types-docker-7.0.0.20240529/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:25:23.659215 types-docker-7.0.0.20240529/docker-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-29 02:25:21.000000 types-docker-7.0.0.20240529/docker-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:25:23.663215 types-docker-7.0.0.20240529/docker-stubs/api/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/api/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/api/build.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/api/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/api/config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6926 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/api/container.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/api/daemon.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/api/exec_api.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/api/image.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/api/network.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/api/plugin.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/api/secret.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/api/service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/api/swarm.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/api/volume.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/auth.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/constants.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:25:23.663215 types-docker-7.0.0.20240529/docker-stubs/context/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/context/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/context/api.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/context/config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/context/context.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:25:23.663215 types-docker-7.0.0.20240529/docker-stubs/credentials/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/credentials/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/credentials/constants.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/credentials/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/credentials/store.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/credentials/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/errors.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:25:23.667215 types-docker-7.0.0.20240529/docker-stubs/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/models/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/models/configs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/models/containers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/models/images.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/models/networks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/models/nodes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/models/plugins.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/models/resource.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/models/secrets.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/models/services.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/models/swarm.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/models/volumes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 02:25:21.000000 types-docker-7.0.0.20240529/docker-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/tls.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:25:23.667215 types-docker-7.0.0.20240529/docker-stubs/transport/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/transport/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/transport/basehttpadapter.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/transport/npipeconn.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/transport/npipesocket.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/transport/sshconn.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/transport/unixconn.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:25:23.667215 types-docker-7.0.0.20240529/docker-stubs/types/
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/types/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/types/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/types/containers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/types/daemon.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/types/healthcheck.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/types/networks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/types/services.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/types/swarm.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:25:23.671215 types-docker-7.0.0.20240529/docker-stubs/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/utils/build.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/utils/config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/utils/decorators.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/utils/fnmatch.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/utils/json_stream.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/utils/ports.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/utils/proxy.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/utils/socket.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/utils/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-29 02:25:11.000000 types-docker-7.0.0.20240529/docker-stubs/version.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 02:25:23.671215 types-docker-7.0.0.20240529/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-05-29 02:25:21.000000 types-docker-7.0.0.20240529/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:25:23.671215 types-docker-7.0.0.20240529/types_docker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-29 02:25:23.000000 types-docker-7.0.0.20240529/types_docker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-29 02:25:23.000000 types-docker-7.0.0.20240529/types_docker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 02:25:23.000000 types-docker-7.0.0.20240529/types_docker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-29 02:25:23.000000 types-docker-7.0.0.20240529/types_docker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-29 02:25:23.000000 types-docker-7.0.0.20240529/types_docker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:27:29.119122 types-docker-7.1.0.20240601/
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-06-01 02:27:28.000000 types-docker-7.1.0.20240601/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-06-01 02:27:28.000000 types-docker-7.1.0.20240601/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-06-01 02:27:29.119122 types-docker-7.1.0.20240601/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:27:29.111122 types-docker-7.1.0.20240601/docker-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-06-01 02:27:28.000000 types-docker-7.1.0.20240601/docker-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:27:29.115122 types-docker-7.1.0.20240601/docker-stubs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/api/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/api/build.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/api/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/api/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6926 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/api/container.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/api/daemon.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/api/exec_api.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/api/image.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/api/network.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/api/plugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/api/secret.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/api/service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/api/swarm.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/api/volume.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/auth.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/constants.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:27:29.115122 types-docker-7.1.0.20240601/docker-stubs/context/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/context/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/context/api.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/context/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/context/context.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:27:29.115122 types-docker-7.1.0.20240601/docker-stubs/credentials/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/credentials/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/credentials/constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/credentials/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/credentials/store.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/credentials/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/errors.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:27:29.115122 types-docker-7.1.0.20240601/docker-stubs/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/models/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/models/configs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/models/containers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/models/images.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/models/networks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/models/nodes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/models/plugins.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/models/resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/models/secrets.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/models/services.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/models/swarm.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/models/volumes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 02:27:28.000000 types-docker-7.1.0.20240601/docker-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/tls.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:27:29.119122 types-docker-7.1.0.20240601/docker-stubs/transport/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/transport/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/transport/basehttpadapter.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/transport/npipeconn.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/transport/npipesocket.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/transport/sshconn.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/transport/unixconn.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:27:29.119122 types-docker-7.1.0.20240601/docker-stubs/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/types/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/types/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/types/containers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/types/daemon.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/types/healthcheck.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/types/networks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/types/services.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/types/swarm.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:27:29.119122 types-docker-7.1.0.20240601/docker-stubs/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/utils/build.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/utils/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/utils/decorators.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/utils/fnmatch.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/utils/json_stream.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/utils/ports.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/utils/proxy.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/utils/socket.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/utils/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-06-01 02:27:05.000000 types-docker-7.1.0.20240601/docker-stubs/version.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 02:27:29.119122 types-docker-7.1.0.20240601/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-06-01 02:27:28.000000 types-docker-7.1.0.20240601/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:27:29.119122 types-docker-7.1.0.20240601/types_docker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-06-01 02:27:29.000000 types-docker-7.1.0.20240601/types_docker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-06-01 02:27:29.000000 types-docker-7.1.0.20240601/types_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 02:27:29.000000 types-docker-7.1.0.20240601/types_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-06-01 02:27:29.000000 types-docker-7.1.0.20240601/types_docker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-01 02:27:29.000000 types-docker-7.1.0.20240601/types_docker.egg-info/top_level.txt
```

### Comparing `types-docker-7.0.0.20240529/CHANGELOG.md` & `types-docker-7.1.0.20240601/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 7.1.0.20240601 (2024-06-01)
+
+[docker] Annotate Container.stop() (#12052)
+
+Update docker to 7.1.x (#12068)
+
 ## 7.0.0.20240529 (2024-05-29)
 
 Add types to docker.models.containers.Container.logs (#12044)
 
 ## 7.0.0.20240528 (2024-05-28)
 
 Add keyword argument types to `docker.models.containers.Container.wait()` (#12037)
```

### Comparing `types-docker-7.0.0.20240529/PKG-INFO` & `types-docker-7.1.0.20240601/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-docker
-Version: 7.0.0.20240529
+Version: 7.1.0.20240601
 Summary: Typing stubs for docker
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/docker.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,16 +22,16 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `docker`.
 
 This version of `types-docker` aims to provide accurate annotations
-for `docker==7.0.*`.
+for `docker==7.1.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/docker. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `b2f6e5221b180d42a3770543a72036baa52b3907` and was tested
-with mypy 1.10.0, pyright 1.1.364, and
+This package was generated from typeshed commit `4b6558c12ac43cd40716cd6452fe98a632ae65d7` and was tested
+with mypy 1.10.0, pyright 1.1.365, and
 pytype 2024.4.11.
```

### Comparing `types-docker-7.0.0.20240529/docker-stubs/api/build.pyi` & `types-docker-7.1.0.20240601/docker-stubs/api/build.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240529/docker-stubs/api/client.pyi` & `types-docker-7.1.0.20240601/docker-stubs/api/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     credstore_env: Mapping[Incomplete, Incomplete] | None
     def __init__(
         self,
         base_url: str | None = None,
         version: str | None = None,
         timeout: int = 60,
         tls: bool | TLSConfig = False,
-        user_agent: str = "docker-sdk-python/7.0.0",
+        user_agent: str = ...,
         num_pools: int | None = None,
         credstore_env: Mapping[Incomplete, Incomplete] | None = None,
         use_ssh_client: bool = False,
         max_pool_size: int = 10,
     ) -> None: ...
     def get_adapter(self, url: str) -> BaseAdapter: ...
     @property
```

### Comparing `types-docker-7.0.0.20240529/docker-stubs/api/container.pyi` & `types-docker-7.1.0.20240601/docker-stubs/api/container.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240529/docker-stubs/api/daemon.pyi` & `types-docker-7.1.0.20240601/docker-stubs/api/daemon.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240529/docker-stubs/api/exec_api.pyi` & `types-docker-7.1.0.20240601/docker-stubs/api/exec_api.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240529/docker-stubs/api/image.pyi` & `types-docker-7.1.0.20240601/docker-stubs/api/image.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240529/docker-stubs/api/network.pyi` & `types-docker-7.1.0.20240601/docker-stubs/api/network.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240529/docker-stubs/api/plugin.pyi` & `types-docker-7.1.0.20240601/docker-stubs/api/plugin.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240529/docker-stubs/api/service.pyi` & `types-docker-7.1.0.20240601/docker-stubs/api/service.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240529/docker-stubs/api/swarm.pyi` & `types-docker-7.1.0.20240601/docker-stubs/api/swarm.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240529/docker-stubs/api/volume.pyi` & `types-docker-7.1.0.20240601/docker-stubs/api/volume.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240529/docker-stubs/auth.pyi` & `types-docker-7.1.0.20240601/docker-stubs/auth.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240529/docker-stubs/client.pyi` & `types-docker-7.1.0.20240601/docker-stubs/client.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240529/docker-stubs/constants.pyi` & `types-docker-7.1.0.20240601/docker-stubs/constants.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240529/docker-stubs/context/api.pyi` & `types-docker-7.1.0.20240601/docker-stubs/context/api.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240529/docker-stubs/context/context.pyi` & `types-docker-7.1.0.20240601/docker-stubs/context/context.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240529/docker-stubs/errors.pyi` & `types-docker-7.1.0.20240601/docker-stubs/errors.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240529/docker-stubs/models/containers.pyi` & `types-docker-7.1.0.20240601/docker-stubs/models/containers.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     def put_archive(self, path: str, data) -> bool: ...
     def remove(self, **kwargs) -> None: ...
     def rename(self, name: str): ...
     def resize(self, height: int, width: int): ...
     def restart(self, **kwargs): ...
     def start(self, **kwargs) -> None: ...
     def stats(self, **kwargs): ...
-    def stop(self, **kwargs) -> None: ...
+    def stop(self, *, timeout: float | None = None) -> None: ...
     def top(self, **kwargs): ...
     def unpause(self): ...
     def update(self, **kwargs): ...
     def wait(self, *, timeout: float | None = None, condition: Literal["not-running", "next-exit", "removed"] | None = None): ...
 
 class ContainerCollection(Collection[Container]):
     model: type[Container]
```

### Comparing `types-docker-7.0.0.20240529/docker-stubs/models/images.pyi` & `types-docker-7.1.0.20240601/docker-stubs/models/images.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240529/docker-stubs/models/networks.pyi` & `types-docker-7.1.0.20240601/docker-stubs/models/networks.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240529/docker-stubs/models/plugins.pyi` & `types-docker-7.1.0.20240601/docker-stubs/models/plugins.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240529/docker-stubs/models/resource.pyi` & `types-docker-7.1.0.20240601/docker-stubs/models/resource.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240529/docker-stubs/models/services.pyi` & `types-docker-7.1.0.20240601/docker-stubs/models/services.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240529/docker-stubs/models/swarm.pyi` & `types-docker-7.1.0.20240601/docker-stubs/models/swarm.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240529/docker-stubs/models/volumes.pyi` & `types-docker-7.1.0.20240601/docker-stubs/models/volumes.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240529/docker-stubs/transport/npipeconn.pyi` & `types-docker-7.1.0.20240601/docker-stubs/transport/npipeconn.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240529/docker-stubs/transport/npipesocket.pyi` & `types-docker-7.1.0.20240601/docker-stubs/transport/npipesocket.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240529/docker-stubs/transport/sshconn.pyi` & `types-docker-7.1.0.20240601/docker-stubs/transport/sshconn.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240529/docker-stubs/transport/unixconn.pyi` & `types-docker-7.1.0.20240601/docker-stubs/transport/unixconn.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240529/docker-stubs/types/__init__.pyi` & `types-docker-7.1.0.20240601/docker-stubs/types/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240529/docker-stubs/types/containers.pyi` & `types-docker-7.1.0.20240601/docker-stubs/types/containers.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240529/docker-stubs/types/healthcheck.pyi` & `types-docker-7.1.0.20240601/docker-stubs/types/healthcheck.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240529/docker-stubs/types/networks.pyi` & `types-docker-7.1.0.20240601/docker-stubs/types/networks.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240529/docker-stubs/types/services.pyi` & `types-docker-7.1.0.20240601/docker-stubs/types/services.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240529/docker-stubs/types/swarm.pyi` & `types-docker-7.1.0.20240601/docker-stubs/types/swarm.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240529/docker-stubs/utils/__init__.pyi` & `types-docker-7.1.0.20240601/docker-stubs/utils/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240529/docker-stubs/utils/build.pyi` & `types-docker-7.1.0.20240601/docker-stubs/utils/build.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240529/docker-stubs/utils/json_stream.pyi` & `types-docker-7.1.0.20240601/docker-stubs/utils/json_stream.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240529/docker-stubs/utils/proxy.pyi` & `types-docker-7.1.0.20240601/docker-stubs/utils/proxy.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240529/docker-stubs/utils/socket.pyi` & `types-docker-7.1.0.20240601/docker-stubs/utils/socket.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240529/docker-stubs/utils/utils.pyi` & `types-docker-7.1.0.20240601/docker-stubs/utils/utils.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240529/setup.py` & `types-docker-7.1.0.20240601/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,27 +11,27 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `docker`.
 
 This version of `types-docker` aims to provide accurate annotations
-for `docker==7.0.*`.
+for `docker==7.1.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/docker. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `b2f6e5221b180d42a3770543a72036baa52b3907` and was tested
-with mypy 1.10.0, pyright 1.1.364, and
+This package was generated from typeshed commit `4b6558c12ac43cd40716cd6452fe98a632ae65d7` and was tested
+with mypy 1.10.0, pyright 1.1.365, and
 pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="7.0.0.20240529",
+      version="7.1.0.20240601",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/docker.md",
```

### Comparing `types-docker-7.0.0.20240529/types_docker.egg-info/PKG-INFO` & `types-docker-7.1.0.20240601/types_docker.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-docker
-Version: 7.0.0.20240529
+Version: 7.1.0.20240601
 Summary: Typing stubs for docker
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/docker.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,16 +22,16 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `docker`.
 
 This version of `types-docker` aims to provide accurate annotations
-for `docker==7.0.*`.
+for `docker==7.1.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/docker. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `b2f6e5221b180d42a3770543a72036baa52b3907` and was tested
-with mypy 1.10.0, pyright 1.1.364, and
+This package was generated from typeshed commit `4b6558c12ac43cd40716cd6452fe98a632ae65d7` and was tested
+with mypy 1.10.0, pyright 1.1.365, and
 pytype 2024.4.11.
```

### Comparing `types-docker-7.0.0.20240529/types_docker.egg-info/SOURCES.txt` & `types-docker-7.1.0.20240601/types_docker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

