# Comparing `tmp/solver-multiRPC-2.0.3.tar.gz` & `tmp/solver-multiRPC-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solver-multiRPC-2.0.3.tar", last modified: Tue May 14 12:15:44 2024, max compression
+gzip compressed data, was "solver-multiRPC-2.0.4.tar", last modified: Sat Jun  1 15:02:50 2024, max compression
```

## Comparing `solver-multiRPC-2.0.3.tar` & `solver-multiRPC-2.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 mba       (1000) mba       (1000)        0 2024-05-14 12:15:44.387063 solver-multiRPC-2.0.3/
--rw-r--r--   0 mba       (1000) mba       (1000)     3455 2024-05-14 12:15:44.387063 solver-multiRPC-2.0.3/PKG-INFO
--rw-rw-r--   0 mba       (1000) mba       (1000)     2955 2024-04-21 14:40:19.000000 solver-multiRPC-2.0.3/README.md
--rw-rw-r--   0 mba       (1000) mba       (1000)      103 2024-01-30 13:14:22.000000 solver-multiRPC-2.0.3/pyproject.toml
--rw-rw-r--   0 mba       (1000) mba       (1000)      582 2024-05-14 12:15:44.387063 solver-multiRPC-2.0.3/setup.cfg
--rw-rw-r--   0 mba       (1000) mba       (1000)      376 2024-05-14 12:14:23.000000 solver-multiRPC-2.0.3/setup.py
-drwxrwxr-x   0 mba       (1000) mba       (1000)        0 2024-05-14 12:15:44.383063 solver-multiRPC-2.0.3/src/
-drwxrwxr-x   0 mba       (1000) mba       (1000)        0 2024-05-14 12:15:44.387063 solver-multiRPC-2.0.3/src/multirpc/
--rw-rw-r--   0 mba       (1000) mba       (1000)       51 2024-01-30 13:14:22.000000 solver-multiRPC-2.0.3/src/multirpc/__init__.py
--rw-rw-r--   0 mba       (1000) mba       (1000)     4348 2024-05-14 11:18:19.000000 solver-multiRPC-2.0.3/src/multirpc/async_multi_rpc_interface.py
--rw-rw-r--   0 mba       (1000) mba       (1000)    22692 2024-05-14 11:18:19.000000 solver-multiRPC-2.0.3/src/multirpc/base_multi_rpc_interface.py
--rw-rw-r--   0 mba       (1000) mba       (1000)      608 2024-05-14 11:18:19.000000 solver-multiRPC-2.0.3/src/multirpc/constants.py
--rw-rw-r--   0 mba       (1000) mba       (1000)     1351 2024-05-14 11:18:19.000000 solver-multiRPC-2.0.3/src/multirpc/exceptions.py
--rw-rw-r--   0 mba       (1000) mba       (1000)     6620 2024-05-14 11:16:22.000000 solver-multiRPC-2.0.3/src/multirpc/gas_estimation.py
--rw-rw-r--   0 mba       (1000) mba       (1000)     4618 2024-05-14 11:18:21.000000 solver-multiRPC-2.0.3/src/multirpc/sync_multi_rpc_interface.py
--rw-rw-r--   0 mba       (1000) mba       (1000)     7243 2024-05-14 11:18:19.000000 solver-multiRPC-2.0.3/src/multirpc/tx_trace.py
--rw-rw-r--   0 mba       (1000) mba       (1000)     5010 2024-05-14 11:18:23.000000 solver-multiRPC-2.0.3/src/multirpc/utils.py
-drwxrwxr-x   0 mba       (1000) mba       (1000)        0 2024-05-14 12:15:44.387063 solver-multiRPC-2.0.3/src/solver_multiRPC.egg-info/
--rw-r--r--   0 mba       (1000) mba       (1000)     3455 2024-05-14 12:15:44.000000 solver-multiRPC-2.0.3/src/solver_multiRPC.egg-info/PKG-INFO
--rw-rw-r--   0 mba       (1000) mba       (1000)      537 2024-05-14 12:15:44.000000 solver-multiRPC-2.0.3/src/solver_multiRPC.egg-info/SOURCES.txt
--rw-rw-r--   0 mba       (1000) mba       (1000)        1 2024-05-14 12:15:44.000000 solver-multiRPC-2.0.3/src/solver_multiRPC.egg-info/dependency_links.txt
--rw-rw-r--   0 mba       (1000) mba       (1000)        9 2024-05-14 12:15:44.000000 solver-multiRPC-2.0.3/src/solver_multiRPC.egg-info/requires.txt
--rw-rw-r--   0 mba       (1000) mba       (1000)        9 2024-05-14 12:15:44.000000 solver-multiRPC-2.0.3/src/solver_multiRPC.egg-info/top_level.txt
+drwxrwxr-x   0 mba       (1000) mba       (1000)        0 2024-06-01 15:02:50.398765 solver-multiRPC-2.0.4/
+-rw-r--r--   0 mba       (1000) mba       (1000)     3455 2024-06-01 15:02:50.398765 solver-multiRPC-2.0.4/PKG-INFO
+-rw-rw-r--   0 mba       (1000) mba       (1000)     2955 2024-04-21 14:40:19.000000 solver-multiRPC-2.0.4/README.md
+-rw-rw-r--   0 mba       (1000) mba       (1000)      259 2024-06-01 15:02:23.000000 solver-multiRPC-2.0.4/pyproject.toml
+-rw-rw-r--   0 mba       (1000) mba       (1000)      582 2024-06-01 15:02:50.398765 solver-multiRPC-2.0.4/setup.cfg
+-rw-rw-r--   0 mba       (1000) mba       (1000)      376 2024-06-01 15:02:47.000000 solver-multiRPC-2.0.4/setup.py
+drwxrwxr-x   0 mba       (1000) mba       (1000)        0 2024-06-01 15:02:50.394765 solver-multiRPC-2.0.4/src/
+drwxrwxr-x   0 mba       (1000) mba       (1000)        0 2024-06-01 15:02:50.398765 solver-multiRPC-2.0.4/src/multirpc/
+-rw-rw-r--   0 mba       (1000) mba       (1000)       51 2024-01-30 13:14:22.000000 solver-multiRPC-2.0.4/src/multirpc/__init__.py
+-rw-rw-r--   0 mba       (1000) mba       (1000)     4348 2024-05-14 11:18:19.000000 solver-multiRPC-2.0.4/src/multirpc/async_multi_rpc_interface.py
+-rw-rw-r--   0 mba       (1000) mba       (1000)    22693 2024-06-01 15:02:23.000000 solver-multiRPC-2.0.4/src/multirpc/base_multi_rpc_interface.py
+-rw-rw-r--   0 mba       (1000) mba       (1000)      608 2024-05-14 11:18:19.000000 solver-multiRPC-2.0.4/src/multirpc/constants.py
+-rw-rw-r--   0 mba       (1000) mba       (1000)     1351 2024-05-14 11:18:19.000000 solver-multiRPC-2.0.4/src/multirpc/exceptions.py
+-rw-rw-r--   0 mba       (1000) mba       (1000)     6620 2024-05-14 11:16:22.000000 solver-multiRPC-2.0.4/src/multirpc/gas_estimation.py
+-rw-rw-r--   0 mba       (1000) mba       (1000)     4618 2024-06-01 13:36:20.000000 solver-multiRPC-2.0.4/src/multirpc/sync_multi_rpc_interface.py
+-rw-rw-r--   0 mba       (1000) mba       (1000)     7243 2024-05-14 11:18:19.000000 solver-multiRPC-2.0.4/src/multirpc/tx_trace.py
+-rw-rw-r--   0 mba       (1000) mba       (1000)     5027 2024-06-01 13:36:20.000000 solver-multiRPC-2.0.4/src/multirpc/utils.py
+drwxrwxr-x   0 mba       (1000) mba       (1000)        0 2024-06-01 15:02:50.398765 solver-multiRPC-2.0.4/src/solver_multiRPC.egg-info/
+-rw-r--r--   0 mba       (1000) mba       (1000)     3455 2024-06-01 15:02:50.000000 solver-multiRPC-2.0.4/src/solver_multiRPC.egg-info/PKG-INFO
+-rw-rw-r--   0 mba       (1000) mba       (1000)      537 2024-06-01 15:02:50.000000 solver-multiRPC-2.0.4/src/solver_multiRPC.egg-info/SOURCES.txt
+-rw-rw-r--   0 mba       (1000) mba       (1000)        1 2024-06-01 15:02:50.000000 solver-multiRPC-2.0.4/src/solver_multiRPC.egg-info/dependency_links.txt
+-rw-rw-r--   0 mba       (1000) mba       (1000)        9 2024-06-01 15:02:50.000000 solver-multiRPC-2.0.4/src/solver_multiRPC.egg-info/requires.txt
+-rw-rw-r--   0 mba       (1000) mba       (1000)        9 2024-06-01 15:02:50.000000 solver-multiRPC-2.0.4/src/solver_multiRPC.egg-info/top_level.txt
```

### Comparing `solver-multiRPC-2.0.3/PKG-INFO` & `solver-multiRPC-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solver-multiRPC
-Version: 2.0.3
+Version: 2.0.4
 Summary: Use multiple rpc for reliability
 Home-page: https://github.com/SYMM-IO/solver-multiRPC.git
 Author: rorschach
 Author-email: rorschach45001@gmail.com
 Project-URL: Bug Tracker, https://github.com/SYMM-IO/solver-multiRPC
 Keywords: multiRPC solver
 Classifier: Programming Language :: Python :: 3
```

### Comparing `solver-multiRPC-2.0.3/README.md` & `solver-multiRPC-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `solver-multiRPC-2.0.3/setup.cfg` & `solver-multiRPC-2.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `solver-multiRPC-2.0.3/src/multirpc/async_multi_rpc_interface.py` & `solver-multiRPC-2.0.4/src/multirpc/async_multi_rpc_interface.py`

 * *Files identical despite different names*

### Comparing `solver-multiRPC-2.0.3/src/multirpc/base_multi_rpc_interface.py` & `solver-multiRPC-2.0.4/src/multirpc/base_multi_rpc_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -392,15 +392,15 @@
         signed_transaction = await self._build_and_sign_transaction(
             contracts[0], providers[0], func_name, func_args, func_kwargs, private_key, tx_params, enable_gas_estimation
         )
         tx_hash = Web3.to_hex(signed_transaction.hash)
         self._logger_params(tx_hash=tx_hash)
 
         execution_tx_list = [
-            self._send_transaction(p, signed_transaction.rawTransaction) for p in providers
+            self._send_transaction(p, signed_transaction.raw_transaction) for p in providers
         ]
         result = await self.__execute_batch_tasks(
             execution_tx_list,
             [TransactionValueError],
             FailedOnAllRPCs
         )
         provider, tx = result
```

### Comparing `solver-multiRPC-2.0.3/src/multirpc/constants.py` & `solver-multiRPC-2.0.4/src/multirpc/constants.py`

 * *Files identical despite different names*

### Comparing `solver-multiRPC-2.0.3/src/multirpc/exceptions.py` & `solver-multiRPC-2.0.4/src/multirpc/exceptions.py`

 * *Files identical despite different names*

### Comparing `solver-multiRPC-2.0.3/src/multirpc/gas_estimation.py` & `solver-multiRPC-2.0.4/src/multirpc/gas_estimation.py`

 * *Files identical despite different names*

### Comparing `solver-multiRPC-2.0.3/src/multirpc/sync_multi_rpc_interface.py` & `solver-multiRPC-2.0.4/src/multirpc/sync_multi_rpc_interface.py`

 * *Files identical despite different names*

### Comparing `solver-multiRPC-2.0.3/src/multirpc/tx_trace.py` & `solver-multiRPC-2.0.4/src/multirpc/tx_trace.py`

 * *Files identical despite different names*

### Comparing `solver-multiRPC-2.0.3/src/multirpc/utils.py` & `solver-multiRPC-2.0.4/src/multirpc/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import asyncio
 import enum
 import json
 import logging
+import threading
 import time
 from functools import reduce, wraps
 from threading import Thread
 from typing import Dict, List, Tuple, Union
 
 import aiohttp.client_exceptions
 import web3
```

### Comparing `solver-multiRPC-2.0.3/src/solver_multiRPC.egg-info/PKG-INFO` & `solver-multiRPC-2.0.4/src/solver_multiRPC.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solver-multiRPC
-Version: 2.0.3
+Version: 2.0.4
 Summary: Use multiple rpc for reliability
 Home-page: https://github.com/SYMM-IO/solver-multiRPC.git
 Author: rorschach
 Author-email: rorschach45001@gmail.com
 Project-URL: Bug Tracker, https://github.com/SYMM-IO/solver-multiRPC
 Keywords: multiRPC solver
 Classifier: Programming Language :: Python :: 3
```

### Comparing `solver-multiRPC-2.0.3/src/solver_multiRPC.egg-info/SOURCES.txt` & `solver-multiRPC-2.0.4/src/solver_multiRPC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

