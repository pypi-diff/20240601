# Comparing `tmp/neural_solution-2.4.tar.gz` & `tmp/neural_solution-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neural_solution-2.4.tar", last modified: Fri Dec 15 08:57:51 2023, max compression
+gzip compressed data, was "neural_solution-2.5.1.tar", last modified: Sat Jun  1 08:23:32 2024, max compression
```

## Comparing `neural_solution-2.4.tar` & `neural_solution-2.5.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 08:57:51.126254 neural_solution-2.4/
--rw-r--r--   0 root         (0) root         (0)    11360 2023-12-15 08:47:06.000000 neural_solution-2.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)    12627 2023-12-15 08:57:51.126254 neural_solution-2.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11644 2023-12-15 08:47:06.000000 neural_solution-2.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 08:57:51.122254 neural_solution-2.4/neural_solution/
--rw-r--r--   0 root         (0) root         (0)      647 2023-12-15 08:47:06.000000 neural_solution-2.4/neural_solution/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 08:57:51.126254 neural_solution-2.4/neural_solution/backend/
--rw-r--r--   0 root         (0) root         (0)      899 2023-12-15 08:47:06.000000 neural_solution-2.4/neural_solution/backend/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9281 2023-12-15 08:47:06.000000 neural_solution-2.4/neural_solution/backend/cluster.py
--rw-r--r--   0 root         (0) root         (0)     2704 2023-12-15 08:47:06.000000 neural_solution-2.4/neural_solution/backend/result_monitor.py
--rw-r--r--   0 root         (0) root         (0)     3487 2023-12-15 08:47:06.000000 neural_solution-2.4/neural_solution/backend/runner.py
--rw-r--r--   0 root         (0) root         (0)    13590 2023-12-15 08:47:06.000000 neural_solution-2.4/neural_solution/backend/scheduler.py
--rw-r--r--   0 root         (0) root         (0)     2230 2023-12-15 08:47:06.000000 neural_solution-2.4/neural_solution/backend/task.py
--rw-r--r--   0 root         (0) root         (0)     4259 2023-12-15 08:47:06.000000 neural_solution-2.4/neural_solution/backend/task_db.py
--rw-r--r--   0 root         (0) root         (0)     2477 2023-12-15 08:47:06.000000 neural_solution-2.4/neural_solution/backend/task_monitor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 08:57:51.126254 neural_solution-2.4/neural_solution/backend/utils/
--rw-r--r--   0 root         (0) root         (0)      620 2023-12-15 08:47:06.000000 neural_solution-2.4/neural_solution/backend/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6894 2023-12-15 08:47:06.000000 neural_solution-2.4/neural_solution/backend/utils/utility.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 08:57:51.126254 neural_solution-2.4/neural_solution/bin/
--rw-r--r--   0 root         (0) root         (0)      606 2023-12-15 08:47:06.000000 neural_solution-2.4/neural_solution/bin/__init__.py
--rw-r--r--   0 root         (0) root         (0)      772 2023-12-15 08:47:06.000000 neural_solution-2.4/neural_solution/bin/neural_solution.py
--rw-r--r--   0 root         (0) root         (0)      967 2023-12-15 08:47:06.000000 neural_solution-2.4/neural_solution/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 08:57:51.126254 neural_solution-2.4/neural_solution/frontend/
--rw-r--r--   0 root         (0) root         (0)      615 2023-12-15 08:47:06.000000 neural_solution-2.4/neural_solution/frontend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 08:57:51.126254 neural_solution-2.4/neural_solution/frontend/fastapi/
--rw-r--r--   0 root         (0) root         (0)      607 2023-12-15 08:47:06.000000 neural_solution-2.4/neural_solution/frontend/fastapi/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15367 2023-12-15 08:47:06.000000 neural_solution-2.4/neural_solution/frontend/fastapi/main_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 08:57:51.126254 neural_solution-2.4/neural_solution/frontend/gRPC/
--rw-r--r--   0 root         (0) root         (0)      604 2023-12-15 08:47:06.000000 neural_solution-2.4/neural_solution/frontend/gRPC/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4823 2023-12-15 08:47:06.000000 neural_solution-2.4/neural_solution/frontend/gRPC/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 08:57:51.126254 neural_solution-2.4/neural_solution/frontend/gRPC/proto/
--rw-r--r--   0 root         (0) root         (0)      601 2023-12-15 08:47:06.000000 neural_solution-2.4/neural_solution/frontend/gRPC/proto/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3053 2023-12-15 08:47:06.000000 neural_solution-2.4/neural_solution/frontend/gRPC/proto/neural_solution_pb2.py
--rw-r--r--   0 root         (0) root         (0)    17723 2023-12-15 08:47:06.000000 neural_solution-2.4/neural_solution/frontend/gRPC/proto/neural_solution_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     5710 2023-12-15 08:47:06.000000 neural_solution-2.4/neural_solution/frontend/gRPC/server.py
--rw-r--r--   0 root         (0) root         (0)     2238 2023-12-15 08:47:06.000000 neural_solution-2.4/neural_solution/frontend/task_submitter.py
--rw-r--r--   0 root         (0) root         (0)     5443 2023-12-15 08:47:06.000000 neural_solution-2.4/neural_solution/frontend/user_facing_api.json
--rw-r--r--   0 root         (0) root         (0)     9208 2023-12-15 08:47:06.000000 neural_solution-2.4/neural_solution/frontend/utility.py
--rw-r--r--   0 root         (0) root         (0)    14590 2023-12-15 08:47:06.000000 neural_solution-2.4/neural_solution/launcher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 08:57:51.126254 neural_solution-2.4/neural_solution/scripts/
--rw-r--r--   0 root         (0) root         (0)      696 2023-12-15 08:47:06.000000 neural_solution-2.4/neural_solution/scripts/prepare_deps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 08:57:51.126254 neural_solution-2.4/neural_solution/utils/
--rw-r--r--   0 root         (0) root         (0)      689 2023-12-15 08:47:06.000000 neural_solution-2.4/neural_solution/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4595 2023-12-15 08:47:06.000000 neural_solution-2.4/neural_solution/utils/logger.py
--rw-r--r--   0 root         (0) root         (0)     1987 2023-12-15 08:47:06.000000 neural_solution-2.4/neural_solution/utils/utility.py
--rw-r--r--   0 root         (0) root         (0)      705 2023-12-15 08:47:06.000000 neural_solution-2.4/neural_solution/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 08:57:51.122254 neural_solution-2.4/neural_solution.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12627 2023-12-15 08:57:51.000000 neural_solution-2.4/neural_solution.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1553 2023-12-15 08:57:51.000000 neural_solution-2.4/neural_solution.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-15 08:57:51.000000 neural_solution-2.4/neural_solution.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       77 2023-12-15 08:57:51.000000 neural_solution-2.4/neural_solution.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       90 2023-12-15 08:57:51.000000 neural_solution-2.4/neural_solution.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-12-15 08:57:51.000000 neural_solution-2.4/neural_solution.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2418 2023-12-15 08:47:06.000000 neural_solution-2.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      102 2023-12-15 08:57:51.126254 neural_solution-2.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     7117 2023-12-15 08:47:06.000000 neural_solution-2.4/setup.py
--rw-r--r--   0 root         (0) root         (0)    95719 2023-12-15 08:47:06.000000 neural_solution-2.4/third-party-programs.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:23:32.546538 neural_solution-2.5.1/
+-rw-r--r--   0 root         (0) root         (0)    11360 2024-06-01 08:22:37.000000 neural_solution-2.5.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    15082 2024-06-01 08:23:32.546538 neural_solution-2.5.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14096 2024-06-01 08:22:37.000000 neural_solution-2.5.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:23:32.541538 neural_solution-2.5.1/neural_solution/
+-rw-r--r--   0 root         (0) root         (0)      647 2024-06-01 08:22:38.000000 neural_solution-2.5.1/neural_solution/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:23:32.543538 neural_solution-2.5.1/neural_solution/backend/
+-rw-r--r--   0 root         (0) root         (0)      899 2024-06-01 08:22:38.000000 neural_solution-2.5.1/neural_solution/backend/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9281 2024-06-01 08:22:38.000000 neural_solution-2.5.1/neural_solution/backend/cluster.py
+-rw-r--r--   0 root         (0) root         (0)     2704 2024-06-01 08:22:38.000000 neural_solution-2.5.1/neural_solution/backend/result_monitor.py
+-rw-r--r--   0 root         (0) root         (0)     3487 2024-06-01 08:22:38.000000 neural_solution-2.5.1/neural_solution/backend/runner.py
+-rw-r--r--   0 root         (0) root         (0)    13590 2024-06-01 08:22:38.000000 neural_solution-2.5.1/neural_solution/backend/scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     2230 2024-06-01 08:22:38.000000 neural_solution-2.5.1/neural_solution/backend/task.py
+-rw-r--r--   0 root         (0) root         (0)     4259 2024-06-01 08:22:38.000000 neural_solution-2.5.1/neural_solution/backend/task_db.py
+-rw-r--r--   0 root         (0) root         (0)     2477 2024-06-01 08:22:38.000000 neural_solution-2.5.1/neural_solution/backend/task_monitor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:23:32.543538 neural_solution-2.5.1/neural_solution/backend/utils/
+-rw-r--r--   0 root         (0) root         (0)      620 2024-06-01 08:22:38.000000 neural_solution-2.5.1/neural_solution/backend/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6894 2024-06-01 08:22:38.000000 neural_solution-2.5.1/neural_solution/backend/utils/utility.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:23:32.544538 neural_solution-2.5.1/neural_solution/bin/
+-rw-r--r--   0 root         (0) root         (0)      606 2024-06-01 08:22:38.000000 neural_solution-2.5.1/neural_solution/bin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      772 2024-06-01 08:22:38.000000 neural_solution-2.5.1/neural_solution/bin/neural_solution.py
+-rw-r--r--   0 root         (0) root         (0)      967 2024-06-01 08:22:38.000000 neural_solution-2.5.1/neural_solution/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:23:32.544538 neural_solution-2.5.1/neural_solution/frontend/
+-rw-r--r--   0 root         (0) root         (0)      615 2024-06-01 08:22:38.000000 neural_solution-2.5.1/neural_solution/frontend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:23:32.544538 neural_solution-2.5.1/neural_solution/frontend/fastapi/
+-rw-r--r--   0 root         (0) root         (0)      607 2024-06-01 08:22:38.000000 neural_solution-2.5.1/neural_solution/frontend/fastapi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15495 2024-06-01 08:22:38.000000 neural_solution-2.5.1/neural_solution/frontend/fastapi/main_server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:23:32.545538 neural_solution-2.5.1/neural_solution/frontend/gRPC/
+-rw-r--r--   0 root         (0) root         (0)      604 2024-06-01 08:22:38.000000 neural_solution-2.5.1/neural_solution/frontend/gRPC/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4823 2024-06-01 08:22:38.000000 neural_solution-2.5.1/neural_solution/frontend/gRPC/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:23:32.545538 neural_solution-2.5.1/neural_solution/frontend/gRPC/proto/
+-rw-r--r--   0 root         (0) root         (0)      601 2024-06-01 08:22:38.000000 neural_solution-2.5.1/neural_solution/frontend/gRPC/proto/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3053 2024-06-01 08:22:38.000000 neural_solution-2.5.1/neural_solution/frontend/gRPC/proto/neural_solution_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    17723 2024-06-01 08:22:38.000000 neural_solution-2.5.1/neural_solution/frontend/gRPC/proto/neural_solution_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     5710 2024-06-01 08:22:38.000000 neural_solution-2.5.1/neural_solution/frontend/gRPC/server.py
+-rw-r--r--   0 root         (0) root         (0)     2238 2024-06-01 08:22:38.000000 neural_solution-2.5.1/neural_solution/frontend/task_submitter.py
+-rw-r--r--   0 root         (0) root         (0)     5443 2024-06-01 08:22:38.000000 neural_solution-2.5.1/neural_solution/frontend/user_facing_api.json
+-rw-r--r--   0 root         (0) root         (0)    10838 2024-06-01 08:22:38.000000 neural_solution-2.5.1/neural_solution/frontend/utility.py
+-rw-r--r--   0 root         (0) root         (0)    14590 2024-06-01 08:22:38.000000 neural_solution-2.5.1/neural_solution/launcher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:23:32.545538 neural_solution-2.5.1/neural_solution/scripts/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-06-01 08:22:38.000000 neural_solution-2.5.1/neural_solution/scripts/prepare_deps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:23:32.546538 neural_solution-2.5.1/neural_solution/utils/
+-rw-r--r--   0 root         (0) root         (0)      689 2024-06-01 08:22:38.000000 neural_solution-2.5.1/neural_solution/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4595 2024-06-01 08:22:38.000000 neural_solution-2.5.1/neural_solution/utils/logger.py
+-rw-r--r--   0 root         (0) root         (0)     1987 2024-06-01 08:22:38.000000 neural_solution-2.5.1/neural_solution/utils/utility.py
+-rw-r--r--   0 root         (0) root         (0)      705 2024-06-01 08:22:38.000000 neural_solution-2.5.1/neural_solution/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:23:32.546538 neural_solution-2.5.1/neural_solution.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15082 2024-06-01 08:23:32.000000 neural_solution-2.5.1/neural_solution.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1553 2024-06-01 08:23:32.000000 neural_solution-2.5.1/neural_solution.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-01 08:23:32.000000 neural_solution-2.5.1/neural_solution.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       77 2024-06-01 08:23:32.000000 neural_solution-2.5.1/neural_solution.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2024-06-01 08:23:32.000000 neural_solution-2.5.1/neural_solution.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-06-01 08:23:32.000000 neural_solution-2.5.1/neural_solution.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2418 2024-06-01 08:22:38.000000 neural_solution-2.5.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      102 2024-06-01 08:23:32.547538 neural_solution-2.5.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8675 2024-06-01 08:22:38.000000 neural_solution-2.5.1/setup.py
+-rw-r--r--   0 root         (0) root         (0)    95740 2024-06-01 08:22:38.000000 neural_solution-2.5.1/third-party-programs.txt
```

### Comparing `neural_solution-2.4/LICENSE` & `neural_solution-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neural_solution-2.4/PKG-INFO` & `neural_solution-2.5.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,109 +1,135 @@
-Metadata-Version: 2.1
-Name: neural_solution
-Version: 2.4
-Summary: Repository of Intel® Neural Compressor
-Home-page: https://github.com/intel/neural-compressor
-Author: Intel AIA Team
-Author-email: feng.tian@intel.com, haihao.shen@intel.com, suyue.chen@intel.com
-License: Apache 2.0
-Keywords: quantization,auto-tuning,post-training static quantization,post-training dynamic quantization,quantization-aware training
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: third-party-programs.txt
-Requires-Dist: fastapi
-Requires-Dist: grpcio
-Requires-Dist: mpi4py
-Requires-Dist: neural_compressor>=2.2
-Requires-Dist: protobuf
-Requires-Dist: pydantic
-Requires-Dist: uvicorn[standard]
-Requires-Dist: watchdog
-
 <div align="center">
 
 Intel® Neural Compressor
 ===========================
 <h3> An open-source Python library supporting popular model compression techniques on all mainstream deep learning frameworks (TensorFlow, PyTorch, ONNX Runtime, and MXNet)</h3>
 
 [![python](https://img.shields.io/badge/python-3.8%2B-blue)](https://github.com/intel/neural-compressor)
-[![version](https://img.shields.io/badge/release-2.4-green)](https://github.com/intel/neural-compressor/releases)
+[![version](https://img.shields.io/badge/release-2.5-green)](https://github.com/intel/neural-compressor/releases)
 [![license](https://img.shields.io/badge/license-Apache%202-blue)](https://github.com/intel/neural-compressor/blob/master/LICENSE)
 [![coverage](https://img.shields.io/badge/coverage-85%25-green)](https://github.com/intel/neural-compressor)
 [![Downloads](https://static.pepy.tech/personalized-badge/neural-compressor?period=total&units=international_system&left_color=grey&right_color=green&left_text=downloads)](https://pepy.tech/project/neural-compressor)
 
-[Architecture](./docs/source/design.md#architecture)&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;[Workflow](./docs/source/design.md#workflow)&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;[Results](./docs/source/validated_model_list.md)&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;[Examples](./examples/README.md)&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;[Documentations](https://intel.github.io/neural-compressor)
+[Architecture](./docs/source/design.md#architecture)&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;[Workflow](./docs/source/design.md#workflow)&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;[LLMs Recipes](./docs/source/llm_recipes.md)&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;[Results](./docs/source/validated_model_list.md)&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;[Documentations](https://intel.github.io/neural-compressor)
 
 ---
 <div align="left">
 
 Intel® Neural Compressor aims to provide popular model compression techniques such as quantization, pruning (sparsity), distillation, and neural architecture search on mainstream frameworks such as [TensorFlow](https://www.tensorflow.org/), [PyTorch](https://pytorch.org/), [ONNX Runtime](https://onnxruntime.ai/), and [MXNet](https://mxnet.apache.org/),
 as well as Intel extensions such as [Intel Extension for TensorFlow](https://github.com/intel/intel-extension-for-tensorflow) and [Intel Extension for PyTorch](https://github.com/intel/intel-extension-for-pytorch).
 In particular, the tool provides the key features, typical examples, and open collaborations as below:
 
 * Support a wide range of Intel hardware such as [Intel Xeon Scalable Processors](https://www.intel.com/content/www/us/en/products/details/processors/xeon/scalable.html), [Intel Xeon CPU Max Series](https://www.intel.com/content/www/us/en/products/details/processors/xeon/max-series.html), [Intel Data Center GPU Flex Series](https://www.intel.com/content/www/us/en/products/details/discrete-gpus/data-center-gpu/flex-series.html), and [Intel Data Center GPU Max Series](https://www.intel.com/content/www/us/en/products/details/discrete-gpus/data-center-gpu/max-series.html) with extensive testing; support AMD CPU, ARM CPU, and NVidia GPU through ONNX Runtime with limited testing
 
 * Validate popular LLMs such as [LLama2](/examples/pytorch/nlp/huggingface_models/language-modeling/quantization/llm), [Falcon](/examples/pytorch/nlp/huggingface_models/language-modeling/quantization/llm), [GPT-J](/examples/pytorch/nlp/huggingface_models/language-modeling/quantization/llm), [Bloom](/examples/pytorch/nlp/huggingface_models/language-modeling/quantization/llm), [OPT](/examples/pytorch/nlp/huggingface_models/language-modeling/quantization/llm), and more than 10,000 broad models such as [Stable Diffusion](/examples/pytorch/nlp/huggingface_models/text-to-image/quantization), [BERT-Large](/examples/pytorch/nlp/huggingface_models/text-classification/quantization/ptq_static/fx), and [ResNet50](/examples/pytorch/image_recognition/torchvision_models/quantization/ptq/cpu/fx) from popular model hubs such as [Hugging Face](https://huggingface.co/), [Torch Vision](https://pytorch.org/vision/stable/index.html), and [ONNX Model Zoo](https://github.com/onnx/models#models), by leveraging zero-code optimization solution [Neural Coder](/neural_coder#what-do-we-offer) and automatic [accuracy-driven](/docs/source/design.md#workflow) quantization strategies
 
 * Collaborate with cloud marketplaces such as [Google Cloud Platform](https://console.cloud.google.com/marketplace/product/bitnami-launchpad/inc-tensorflow-intel?project=verdant-sensor-286207), [Amazon Web Services](https://aws.amazon.com/marketplace/pp/prodview-yjyh2xmggbmga#pdp-support), and [Azure](https://azuremarketplace.microsoft.com/en-us/marketplace/apps/bitnami.inc-tensorflow-intel), software platforms such as [Alibaba Cloud](https://www.intel.com/content/www/us/en/developer/articles/technical/quantize-ai-by-oneapi-analytics-on-alibaba-cloud.html), [Tencent TACO](https://new.qq.com/rain/a/20221202A00B9S00) and [Microsoft Olive](https://github.com/microsoft/Olive), and open AI ecosystem such as [Hugging Face](https://huggingface.co/blog/intel), [PyTorch](https://pytorch.org/tutorials/recipes/intel_neural_compressor_for_pytorch.html), [ONNX](https://github.com/onnx/models#models), [ONNX Runtime](https://github.com/microsoft/onnxruntime), and [Lightning AI](https://github.com/Lightning-AI/lightning/blob/master/docs/source-pytorch/advanced/post_training_quantization.rst)
 
+## What's New
+* [2024/03] A new SOTA approach [AutoRound](https://github.com/intel/auto-round) Weight-Only Quantization on [Intel Gaudi2 AI accelerator](https://habana.ai/products/gaudi2/) is available for LLMs.
+
 ## Installation
 
 ### Install from pypi
 ```Shell
 pip install neural-compressor
 ```
 > **Note**: 
 > More installation methods can be found at [Installation Guide](https://github.com/intel/neural-compressor/blob/master/docs/source/installation_guide.md). Please check out our [FAQ](https://github.com/intel/neural-compressor/blob/master/docs/source/faq.md) for more details.
 
 ## Getting Started
-### Quantization with Python API
 
-```shell
-# Install Intel Neural Compressor and TensorFlow
-pip install neural-compressor
-pip install tensorflow
-# Prepare fp32 model
-wget https://storage.googleapis.com/intel-optimized-tensorflow/models/v1_6/mobilenet_v1_1.0_224_frozen.pb
+Setting up the environment:  
+```bash
+pip install "neural-compressor>=2.3" "transformers>=4.34.0" torch torchvision
 ```
+After successfully installing these packages, try your first quantization program.
+
+### Weight-Only Quantization (LLMs)
+Following example code demonstrates Weight-Only Quantization on LLMs, it supports Intel CPU, Intel Gauid2 AI Accelerator, Nvidia GPU, best device will be selected automatically. 
+
+To try on Intel Gaudi2, docker image with Gaudi Software Stack is recommended, please refer to following script for environment setup. More details can be found in [Gaudi Guide](https://docs.habana.ai/en/latest/Installation_Guide/Bare_Metal_Fresh_OS.html#launch-docker-image-that-was-built). 
+```bash
+docker run -it --runtime=habana -e HABANA_VISIBLE_DEVICES=all -e OMPI_MCA_btl_vader_single_copy_mechanism=none --cap-add=sys_nice --net=host --ipc=host vault.habana.ai/gaudi-docker/1.14.0/ubuntu22.04//habanalabs/pytorch-installer-2.1.1:latest
+
+# Check the container ID
+docker ps
+
+# Login into container
+docker exec -it <container_id> bash
+
+# Install the optimum-habana
+pip install --upgrade-strategy eager optimum[habana]
+
+# Install INC/auto_round
+pip install neural-compressor auto_round
+```
+Run the example:
 ```python
-from neural_compressor.data import DataLoader, Datasets
+from transformers import AutoModel, AutoTokenizer
+
 from neural_compressor.config import PostTrainingQuantConfig
+from neural_compressor.quantization import fit
+from neural_compressor.adaptor.torch_utils.auto_round import get_dataloader
+
+model_name = "EleutherAI/gpt-neo-125m"
+float_model = AutoModel.from_pretrained(model_name)
+tokenizer = AutoTokenizer.from_pretrained(model_name, trust_remote_code=True)
+dataloader = get_dataloader(tokenizer, seqlen=2048)
+
+woq_conf = PostTrainingQuantConfig(
+    approach="weight_only",
+    op_type_dict={
+        ".*": {  # match all ops
+            "weight": {
+                "dtype": "int",
+                "bits": 4,
+                "algorithm": "AUTOROUND",
+            },
+        }
+    },
+)
+quantized_model = fit(model=float_model, conf=woq_conf, calib_dataloader=dataloader)
+```
+**Note:** 
+
+To try INT4 model inference, please directly use [Intel Extension for Transformers](https://github.com/intel/intel-extension-for-transformers), which leverages Intel Neural Compressor for model quantization.        
 
-dataset = Datasets("tensorflow")["dummy"](shape=(1, 224, 224, 3))
-dataloader = DataLoader(framework="tensorflow", dataset=dataset)
+### Static Quantization (Non-LLMs)
 
+```python
+from torchvision import models
+
+from neural_compressor.config import PostTrainingQuantConfig
+from neural_compressor.data import DataLoader, Datasets
 from neural_compressor.quantization import fit
 
-q_model = fit(
-    model="./mobilenet_v1_1.0_224_frozen.pb",
-    conf=PostTrainingQuantConfig(),
-    calib_dataloader=dataloader,
-)
+float_model = models.resnet18()
+dataset = Datasets("pytorch")["dummy"](shape=(1, 3, 224, 224))
+calib_dataloader = DataLoader(framework="pytorch", dataset=dataset)
+static_quant_conf = PostTrainingQuantConfig()
+quantized_model = fit(model=float_model, conf=static_quant_conf, calib_dataloader=calib_dataloader)
 ```
 
 ## Documentation
 
 <table class="docutils">
   <thead>
   <tr>
     <th colspan="8">Overview</th>
   </tr>
   </thead>
   <tbody>
     <tr>
       <td colspan="2" align="center"><a href="./docs/source/design.md#architecture">Architecture</a></td>
       <td colspan="2" align="center"><a href="./docs/source/design.md#workflow">Workflow</a></td>
+      <td colspan="1" align="center"><a href="https://intel.github.io/neural-compressor/latest/docs/source/api-doc/apis.html">APIs</a></td>
+      <td colspan="1" align="center"><a href="./docs/source/llm_recipes.md">LLMs Recipes</a></td>
       <td colspan="2" align="center"><a href="examples/README.md">Examples</a></td>
-      <td colspan="2" align="center"><a href="https://intel.github.io/neural-compressor/latest/docs/source/api-doc/apis.html">APIs</a></td>
     </tr>
   </tbody>
   <thead>
     <tr>
       <th colspan="8">Python-based APIs</th>
     </tr>
   </thead>
```

### Comparing `neural_solution-2.4/README.md` & `neural_solution-2.5.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,83 +1,161 @@
+Metadata-Version: 2.1
+Name: neural_solution
+Version: 2.5.1
+Summary: Repository of Intel® Neural Compressor
+Home-page: https://github.com/intel/neural-compressor
+Author: Intel AIPT Team
+Author-email: feng.tian@intel.com, haihao.shen@intel.com, suyue.chen@intel.com
+License: Apache 2.0
+Keywords: quantization,auto-tuning,post-training static quantization,post-training dynamic quantization,quantization-aware training
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: >=3.7.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: third-party-programs.txt
+Requires-Dist: fastapi
+Requires-Dist: grpcio
+Requires-Dist: mpi4py
+Requires-Dist: neural_compressor>=2.2
+Requires-Dist: protobuf
+Requires-Dist: pydantic
+Requires-Dist: uvicorn[standard]
+Requires-Dist: watchdog
+
 <div align="center">
 
 Intel® Neural Compressor
 ===========================
 <h3> An open-source Python library supporting popular model compression techniques on all mainstream deep learning frameworks (TensorFlow, PyTorch, ONNX Runtime, and MXNet)</h3>
 
 [![python](https://img.shields.io/badge/python-3.8%2B-blue)](https://github.com/intel/neural-compressor)
-[![version](https://img.shields.io/badge/release-2.4-green)](https://github.com/intel/neural-compressor/releases)
+[![version](https://img.shields.io/badge/release-2.5-green)](https://github.com/intel/neural-compressor/releases)
 [![license](https://img.shields.io/badge/license-Apache%202-blue)](https://github.com/intel/neural-compressor/blob/master/LICENSE)
 [![coverage](https://img.shields.io/badge/coverage-85%25-green)](https://github.com/intel/neural-compressor)
 [![Downloads](https://static.pepy.tech/personalized-badge/neural-compressor?period=total&units=international_system&left_color=grey&right_color=green&left_text=downloads)](https://pepy.tech/project/neural-compressor)
 
-[Architecture](./docs/source/design.md#architecture)&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;[Workflow](./docs/source/design.md#workflow)&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;[Results](./docs/source/validated_model_list.md)&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;[Examples](./examples/README.md)&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;[Documentations](https://intel.github.io/neural-compressor)
+[Architecture](./docs/source/design.md#architecture)&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;[Workflow](./docs/source/design.md#workflow)&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;[LLMs Recipes](./docs/source/llm_recipes.md)&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;[Results](./docs/source/validated_model_list.md)&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;[Documentations](https://intel.github.io/neural-compressor)
 
 ---
 <div align="left">
 
 Intel® Neural Compressor aims to provide popular model compression techniques such as quantization, pruning (sparsity), distillation, and neural architecture search on mainstream frameworks such as [TensorFlow](https://www.tensorflow.org/), [PyTorch](https://pytorch.org/), [ONNX Runtime](https://onnxruntime.ai/), and [MXNet](https://mxnet.apache.org/),
 as well as Intel extensions such as [Intel Extension for TensorFlow](https://github.com/intel/intel-extension-for-tensorflow) and [Intel Extension for PyTorch](https://github.com/intel/intel-extension-for-pytorch).
 In particular, the tool provides the key features, typical examples, and open collaborations as below:
 
 * Support a wide range of Intel hardware such as [Intel Xeon Scalable Processors](https://www.intel.com/content/www/us/en/products/details/processors/xeon/scalable.html), [Intel Xeon CPU Max Series](https://www.intel.com/content/www/us/en/products/details/processors/xeon/max-series.html), [Intel Data Center GPU Flex Series](https://www.intel.com/content/www/us/en/products/details/discrete-gpus/data-center-gpu/flex-series.html), and [Intel Data Center GPU Max Series](https://www.intel.com/content/www/us/en/products/details/discrete-gpus/data-center-gpu/max-series.html) with extensive testing; support AMD CPU, ARM CPU, and NVidia GPU through ONNX Runtime with limited testing
 
 * Validate popular LLMs such as [LLama2](/examples/pytorch/nlp/huggingface_models/language-modeling/quantization/llm), [Falcon](/examples/pytorch/nlp/huggingface_models/language-modeling/quantization/llm), [GPT-J](/examples/pytorch/nlp/huggingface_models/language-modeling/quantization/llm), [Bloom](/examples/pytorch/nlp/huggingface_models/language-modeling/quantization/llm), [OPT](/examples/pytorch/nlp/huggingface_models/language-modeling/quantization/llm), and more than 10,000 broad models such as [Stable Diffusion](/examples/pytorch/nlp/huggingface_models/text-to-image/quantization), [BERT-Large](/examples/pytorch/nlp/huggingface_models/text-classification/quantization/ptq_static/fx), and [ResNet50](/examples/pytorch/image_recognition/torchvision_models/quantization/ptq/cpu/fx) from popular model hubs such as [Hugging Face](https://huggingface.co/), [Torch Vision](https://pytorch.org/vision/stable/index.html), and [ONNX Model Zoo](https://github.com/onnx/models#models), by leveraging zero-code optimization solution [Neural Coder](/neural_coder#what-do-we-offer) and automatic [accuracy-driven](/docs/source/design.md#workflow) quantization strategies
 
 * Collaborate with cloud marketplaces such as [Google Cloud Platform](https://console.cloud.google.com/marketplace/product/bitnami-launchpad/inc-tensorflow-intel?project=verdant-sensor-286207), [Amazon Web Services](https://aws.amazon.com/marketplace/pp/prodview-yjyh2xmggbmga#pdp-support), and [Azure](https://azuremarketplace.microsoft.com/en-us/marketplace/apps/bitnami.inc-tensorflow-intel), software platforms such as [Alibaba Cloud](https://www.intel.com/content/www/us/en/developer/articles/technical/quantize-ai-by-oneapi-analytics-on-alibaba-cloud.html), [Tencent TACO](https://new.qq.com/rain/a/20221202A00B9S00) and [Microsoft Olive](https://github.com/microsoft/Olive), and open AI ecosystem such as [Hugging Face](https://huggingface.co/blog/intel), [PyTorch](https://pytorch.org/tutorials/recipes/intel_neural_compressor_for_pytorch.html), [ONNX](https://github.com/onnx/models#models), [ONNX Runtime](https://github.com/microsoft/onnxruntime), and [Lightning AI](https://github.com/Lightning-AI/lightning/blob/master/docs/source-pytorch/advanced/post_training_quantization.rst)
 
+## What's New
+* [2024/03] A new SOTA approach [AutoRound](https://github.com/intel/auto-round) Weight-Only Quantization on [Intel Gaudi2 AI accelerator](https://habana.ai/products/gaudi2/) is available for LLMs.
+
 ## Installation
 
 ### Install from pypi
 ```Shell
 pip install neural-compressor
 ```
 > **Note**: 
 > More installation methods can be found at [Installation Guide](https://github.com/intel/neural-compressor/blob/master/docs/source/installation_guide.md). Please check out our [FAQ](https://github.com/intel/neural-compressor/blob/master/docs/source/faq.md) for more details.
 
 ## Getting Started
-### Quantization with Python API
 
-```shell
-# Install Intel Neural Compressor and TensorFlow
-pip install neural-compressor
-pip install tensorflow
-# Prepare fp32 model
-wget https://storage.googleapis.com/intel-optimized-tensorflow/models/v1_6/mobilenet_v1_1.0_224_frozen.pb
+Setting up the environment:  
+```bash
+pip install "neural-compressor>=2.3" "transformers>=4.34.0" torch torchvision
 ```
+After successfully installing these packages, try your first quantization program.
+
+### Weight-Only Quantization (LLMs)
+Following example code demonstrates Weight-Only Quantization on LLMs, it supports Intel CPU, Intel Gauid2 AI Accelerator, Nvidia GPU, best device will be selected automatically. 
+
+To try on Intel Gaudi2, docker image with Gaudi Software Stack is recommended, please refer to following script for environment setup. More details can be found in [Gaudi Guide](https://docs.habana.ai/en/latest/Installation_Guide/Bare_Metal_Fresh_OS.html#launch-docker-image-that-was-built). 
+```bash
+docker run -it --runtime=habana -e HABANA_VISIBLE_DEVICES=all -e OMPI_MCA_btl_vader_single_copy_mechanism=none --cap-add=sys_nice --net=host --ipc=host vault.habana.ai/gaudi-docker/1.14.0/ubuntu22.04//habanalabs/pytorch-installer-2.1.1:latest
+
+# Check the container ID
+docker ps
+
+# Login into container
+docker exec -it <container_id> bash
+
+# Install the optimum-habana
+pip install --upgrade-strategy eager optimum[habana]
+
+# Install INC/auto_round
+pip install neural-compressor auto_round
+```
+Run the example:
 ```python
-from neural_compressor.data import DataLoader, Datasets
+from transformers import AutoModel, AutoTokenizer
+
 from neural_compressor.config import PostTrainingQuantConfig
+from neural_compressor.quantization import fit
+from neural_compressor.adaptor.torch_utils.auto_round import get_dataloader
+
+model_name = "EleutherAI/gpt-neo-125m"
+float_model = AutoModel.from_pretrained(model_name)
+tokenizer = AutoTokenizer.from_pretrained(model_name, trust_remote_code=True)
+dataloader = get_dataloader(tokenizer, seqlen=2048)
+
+woq_conf = PostTrainingQuantConfig(
+    approach="weight_only",
+    op_type_dict={
+        ".*": {  # match all ops
+            "weight": {
+                "dtype": "int",
+                "bits": 4,
+                "algorithm": "AUTOROUND",
+            },
+        }
+    },
+)
+quantized_model = fit(model=float_model, conf=woq_conf, calib_dataloader=dataloader)
+```
+**Note:** 
+
+To try INT4 model inference, please directly use [Intel Extension for Transformers](https://github.com/intel/intel-extension-for-transformers), which leverages Intel Neural Compressor for model quantization.        
 
-dataset = Datasets("tensorflow")["dummy"](shape=(1, 224, 224, 3))
-dataloader = DataLoader(framework="tensorflow", dataset=dataset)
+### Static Quantization (Non-LLMs)
 
+```python
+from torchvision import models
+
+from neural_compressor.config import PostTrainingQuantConfig
+from neural_compressor.data import DataLoader, Datasets
 from neural_compressor.quantization import fit
 
-q_model = fit(
-    model="./mobilenet_v1_1.0_224_frozen.pb",
-    conf=PostTrainingQuantConfig(),
-    calib_dataloader=dataloader,
-)
+float_model = models.resnet18()
+dataset = Datasets("pytorch")["dummy"](shape=(1, 3, 224, 224))
+calib_dataloader = DataLoader(framework="pytorch", dataset=dataset)
+static_quant_conf = PostTrainingQuantConfig()
+quantized_model = fit(model=float_model, conf=static_quant_conf, calib_dataloader=calib_dataloader)
 ```
 
 ## Documentation
 
 <table class="docutils">
   <thead>
   <tr>
     <th colspan="8">Overview</th>
   </tr>
   </thead>
   <tbody>
     <tr>
       <td colspan="2" align="center"><a href="./docs/source/design.md#architecture">Architecture</a></td>
       <td colspan="2" align="center"><a href="./docs/source/design.md#workflow">Workflow</a></td>
+      <td colspan="1" align="center"><a href="https://intel.github.io/neural-compressor/latest/docs/source/api-doc/apis.html">APIs</a></td>
+      <td colspan="1" align="center"><a href="./docs/source/llm_recipes.md">LLMs Recipes</a></td>
       <td colspan="2" align="center"><a href="examples/README.md">Examples</a></td>
-      <td colspan="2" align="center"><a href="https://intel.github.io/neural-compressor/latest/docs/source/api-doc/apis.html">APIs</a></td>
     </tr>
   </tbody>
   <thead>
     <tr>
       <th colspan="8">Python-based APIs</th>
     </tr>
   </thead>
```

### Comparing `neural_solution-2.4/neural_solution/__init__.py` & `neural_solution-2.5.1/neural_solution/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_solution-2.4/neural_solution/backend/__init__.py` & `neural_solution-2.5.1/neural_solution/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_solution-2.4/neural_solution/backend/cluster.py` & `neural_solution-2.5.1/neural_solution/backend/cluster.py`

 * *Files identical despite different names*

### Comparing `neural_solution-2.4/neural_solution/backend/result_monitor.py` & `neural_solution-2.5.1/neural_solution/backend/result_monitor.py`

 * *Files identical despite different names*

### Comparing `neural_solution-2.4/neural_solution/backend/runner.py` & `neural_solution-2.5.1/neural_solution/backend/runner.py`

 * *Files identical despite different names*

### Comparing `neural_solution-2.4/neural_solution/backend/scheduler.py` & `neural_solution-2.5.1/neural_solution/backend/scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
             shutil.copy(script_path, os.path.abspath(self.task_path))
             task.arguments = task.arguments.replace("=dataset", "=" + os.path.join(example_path, "dataset")).replace(
                 "=model", "=" + os.path.join(example_path, "model")
             )
         if not task.optimized:
             # Generate quantization code with Neural Coder API
             neural_coder_cmd = ["python -m neural_coder --enable --approach"]
-            # for users to define approach: "static, ""static_ipex", "dynamic", "auto"
+            # for users to define approach: "static", "static_ipex", "dynamic", "auto"
             approach = task.approach
             neural_coder_cmd.append(approach)
             if is_remote_url(task.script_url):
                 self.script_name = task.script_url.split("/")[-1]
             neural_coder_cmd.append(self.script_name)
             neural_coder_cmd = " ".join(neural_coder_cmd)
             full_cmd = """cd {}\n{}""".format(self.task_path, neural_coder_cmd)
```

### Comparing `neural_solution-2.4/neural_solution/backend/task.py` & `neural_solution-2.5.1/neural_solution/backend/task.py`

 * *Files identical despite different names*

### Comparing `neural_solution-2.4/neural_solution/backend/task_db.py` & `neural_solution-2.5.1/neural_solution/backend/task_db.py`

 * *Files identical despite different names*

### Comparing `neural_solution-2.4/neural_solution/backend/task_monitor.py` & `neural_solution-2.5.1/neural_solution/backend/task_monitor.py`

 * *Files identical despite different names*

### Comparing `neural_solution-2.4/neural_solution/backend/utils/__init__.py` & `neural_solution-2.5.1/neural_solution/backend/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_solution-2.4/neural_solution/backend/utils/utility.py` & `neural_solution-2.5.1/neural_solution/backend/utils/utility.py`

 * *Files identical despite different names*

### Comparing `neural_solution-2.4/neural_solution/bin/__init__.py` & `neural_solution-2.5.1/neural_solution/bin/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_solution-2.4/neural_solution/bin/neural_solution.py` & `neural_solution-2.5.1/neural_solution/bin/neural_solution.py`

 * *Files identical despite different names*

### Comparing `neural_solution-2.4/neural_solution/config.py` & `neural_solution-2.5.1/neural_solution/config.py`

 * *Files identical despite different names*

### Comparing `neural_solution-2.4/neural_solution/frontend/__init__.py` & `neural_solution-2.5.1/neural_solution/frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_solution-2.4/neural_solution/frontend/fastapi/__init__.py` & `neural_solution-2.5.1/neural_solution/frontend/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_solution-2.4/neural_solution/frontend/fastapi/main_server.py` & `neural_solution-2.5.1/neural_solution/frontend/fastapi/main_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from neural_solution.frontend.utility import (
     check_log_exists,
     deserialize,
     get_baseline_during_tuning,
     get_cluster_info,
     get_cluster_table,
     get_res_during_tuning,
+    is_valid_task,
     list_to_string,
     serialize,
 )
 from neural_solution.utils.utility import get_db_path, get_task_log_workspace, get_task_workspace
 
 # Get config from Launcher.sh
 task_monitor_port = None
@@ -149,18 +150,22 @@
             workers: The requested resource unit number
             status: The status of the task: pending/running/done
             result: The result of the task, which is only value-assigned when the task is done
 
     Returns:
         json: status , id of task and messages.
     """
+    if not is_valid_task(task.dict()):
+        raise HTTPException(status_code=422, detail="Invalid task")
+
     msg = "Task submitted successfully"
     status = "successfully"
     # search the current
     db_path = get_db_path(config.workspace)
+
     if os.path.isfile(db_path):
         conn = sqlite3.connect(db_path)
         cursor = conn.cursor()
         task_id = str(uuid.uuid4()).replace("-", "")
         sql = (
             r"insert into task(id, script_url, optimized, arguments, approach, requirements, workers, status)"
             + r" values ('{}', '{}', {}, '{}', '{}', '{}', {}, 'pending')".format(
```

### Comparing `neural_solution-2.4/neural_solution/frontend/gRPC/__init__.py` & `neural_solution-2.5.1/neural_solution/frontend/gRPC/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_solution-2.4/neural_solution/frontend/gRPC/client.py` & `neural_solution-2.5.1/neural_solution/frontend/gRPC/client.py`

 * *Files identical despite different names*

### Comparing `neural_solution-2.4/neural_solution/frontend/gRPC/proto/__init__.py` & `neural_solution-2.5.1/neural_solution/frontend/gRPC/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_solution-2.4/neural_solution/frontend/gRPC/proto/neural_solution_pb2.py` & `neural_solution-2.5.1/neural_solution/frontend/gRPC/proto/neural_solution_pb2.py`

 * *Files identical despite different names*

### Comparing `neural_solution-2.4/neural_solution/frontend/gRPC/proto/neural_solution_pb2_grpc.py` & `neural_solution-2.5.1/neural_solution/frontend/gRPC/proto/neural_solution_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `neural_solution-2.4/neural_solution/frontend/gRPC/server.py` & `neural_solution-2.5.1/neural_solution/frontend/gRPC/server.py`

 * *Files identical despite different names*

### Comparing `neural_solution-2.4/neural_solution/frontend/task_submitter.py` & `neural_solution-2.5.1/neural_solution/frontend/task_submitter.py`

 * *Files identical despite different names*

### Comparing `neural_solution-2.4/neural_solution/frontend/user_facing_api.json` & `neural_solution-2.5.1/neural_solution/frontend/user_facing_api.json`

 * *Files identical despite different names*

### Comparing `neural_solution-2.4/neural_solution/frontend/utility.py` & `neural_solution-2.5.1/neural_solution/frontend/utility.py`

 * *Files 14% similar despite different names*

```diff
@@ -291,7 +291,65 @@
     Args:
         lst (list): strings
 
     Returns:
         str: string
     """
     return " ".join(str(i) for i in lst)
+
+
+def is_invalid_str(to_test_str: str):
+    """Verify whether the to_test_str is valid.
+
+    Args:
+        to_test_str (str): string to be tested.
+
+    Returns:
+        bool: valid or invalid
+    """
+    return any(char in to_test_str for char in [" ", '"', "'", "&", "|", ";", "`", ">"])
+
+
+def is_valid_task(task: dict) -> bool:
+    """Verify whether the task is valid.
+
+    Args:
+        task (dict): task request
+
+    Returns:
+        bool: valid or invalid
+    """
+    required_fields = ["script_url", "optimized", "arguments", "approach", "requirements", "workers"]
+
+    for field in required_fields:
+        if field not in task:
+            return False
+
+    if not isinstance(task["script_url"], str) or is_invalid_str(task["script_url"]):
+        return False
+
+    if (isinstance(task["optimized"], str) and task["optimized"] not in ["True", "False"]) or (
+        not isinstance(task["optimized"], str) and not isinstance(task["optimized"], bool)
+    ):
+        return False
+
+    if not isinstance(task["arguments"], list):
+        return False
+    else:
+        for argument in task["arguments"]:
+            if is_invalid_str(argument):
+                return False
+
+    if not isinstance(task["approach"], str) or task["approach"] not in ["static", "static_ipex", "dynamic", "auto"]:
+        return False
+
+    if not isinstance(task["requirements"], list):
+        return False
+    else:
+        for requirement in task["requirements"]:
+            if is_invalid_str(requirement):
+                return False
+
+    if not isinstance(task["workers"], int) or task["workers"] < 1:
+        return False
+
+    return True
```

### Comparing `neural_solution-2.4/neural_solution/launcher.py` & `neural_solution-2.5.1/neural_solution/launcher.py`

 * *Files identical despite different names*

### Comparing `neural_solution-2.4/neural_solution/scripts/prepare_deps.py` & `neural_solution-2.5.1/neural_solution/scripts/prepare_deps.py`

 * *Files identical despite different names*

### Comparing `neural_solution-2.4/neural_solution/utils/__init__.py` & `neural_solution-2.5.1/neural_solution/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_solution-2.4/neural_solution/utils/logger.py` & `neural_solution-2.5.1/neural_solution/utils/logger.py`

 * *Files identical despite different names*

### Comparing `neural_solution-2.4/neural_solution/utils/utility.py` & `neural_solution-2.5.1/neural_solution/utils/utility.py`

 * *Files identical despite different names*

### Comparing `neural_solution-2.4/neural_solution/version.py` & `neural_solution-2.5.1/neural_solution/version.py`

 * *Files identical despite different names*

### Comparing `neural_solution-2.4/neural_solution.egg-info/PKG-INFO` & `neural_solution-2.5.1/neural_solution.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: neural-solution
-Version: 2.4
+Name: neural_solution
+Version: 2.5.1
 Summary: Repository of Intel® Neural Compressor
 Home-page: https://github.com/intel/neural-compressor
-Author: Intel AIA Team
+Author: Intel AIPT Team
 Author-email: feng.tian@intel.com, haihao.shen@intel.com, suyue.chen@intel.com
 License: Apache 2.0
 Keywords: quantization,auto-tuning,post-training static quantization,post-training dynamic quantization,quantization-aware training
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License
@@ -27,83 +27,135 @@
 <div align="center">
 
 Intel® Neural Compressor
 ===========================
 <h3> An open-source Python library supporting popular model compression techniques on all mainstream deep learning frameworks (TensorFlow, PyTorch, ONNX Runtime, and MXNet)</h3>
 
 [![python](https://img.shields.io/badge/python-3.8%2B-blue)](https://github.com/intel/neural-compressor)
-[![version](https://img.shields.io/badge/release-2.4-green)](https://github.com/intel/neural-compressor/releases)
+[![version](https://img.shields.io/badge/release-2.5-green)](https://github.com/intel/neural-compressor/releases)
 [![license](https://img.shields.io/badge/license-Apache%202-blue)](https://github.com/intel/neural-compressor/blob/master/LICENSE)
 [![coverage](https://img.shields.io/badge/coverage-85%25-green)](https://github.com/intel/neural-compressor)
 [![Downloads](https://static.pepy.tech/personalized-badge/neural-compressor?period=total&units=international_system&left_color=grey&right_color=green&left_text=downloads)](https://pepy.tech/project/neural-compressor)
 
-[Architecture](./docs/source/design.md#architecture)&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;[Workflow](./docs/source/design.md#workflow)&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;[Results](./docs/source/validated_model_list.md)&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;[Examples](./examples/README.md)&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;[Documentations](https://intel.github.io/neural-compressor)
+[Architecture](./docs/source/design.md#architecture)&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;[Workflow](./docs/source/design.md#workflow)&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;[LLMs Recipes](./docs/source/llm_recipes.md)&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;[Results](./docs/source/validated_model_list.md)&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;[Documentations](https://intel.github.io/neural-compressor)
 
 ---
 <div align="left">
 
 Intel® Neural Compressor aims to provide popular model compression techniques such as quantization, pruning (sparsity), distillation, and neural architecture search on mainstream frameworks such as [TensorFlow](https://www.tensorflow.org/), [PyTorch](https://pytorch.org/), [ONNX Runtime](https://onnxruntime.ai/), and [MXNet](https://mxnet.apache.org/),
 as well as Intel extensions such as [Intel Extension for TensorFlow](https://github.com/intel/intel-extension-for-tensorflow) and [Intel Extension for PyTorch](https://github.com/intel/intel-extension-for-pytorch).
 In particular, the tool provides the key features, typical examples, and open collaborations as below:
 
 * Support a wide range of Intel hardware such as [Intel Xeon Scalable Processors](https://www.intel.com/content/www/us/en/products/details/processors/xeon/scalable.html), [Intel Xeon CPU Max Series](https://www.intel.com/content/www/us/en/products/details/processors/xeon/max-series.html), [Intel Data Center GPU Flex Series](https://www.intel.com/content/www/us/en/products/details/discrete-gpus/data-center-gpu/flex-series.html), and [Intel Data Center GPU Max Series](https://www.intel.com/content/www/us/en/products/details/discrete-gpus/data-center-gpu/max-series.html) with extensive testing; support AMD CPU, ARM CPU, and NVidia GPU through ONNX Runtime with limited testing
 
 * Validate popular LLMs such as [LLama2](/examples/pytorch/nlp/huggingface_models/language-modeling/quantization/llm), [Falcon](/examples/pytorch/nlp/huggingface_models/language-modeling/quantization/llm), [GPT-J](/examples/pytorch/nlp/huggingface_models/language-modeling/quantization/llm), [Bloom](/examples/pytorch/nlp/huggingface_models/language-modeling/quantization/llm), [OPT](/examples/pytorch/nlp/huggingface_models/language-modeling/quantization/llm), and more than 10,000 broad models such as [Stable Diffusion](/examples/pytorch/nlp/huggingface_models/text-to-image/quantization), [BERT-Large](/examples/pytorch/nlp/huggingface_models/text-classification/quantization/ptq_static/fx), and [ResNet50](/examples/pytorch/image_recognition/torchvision_models/quantization/ptq/cpu/fx) from popular model hubs such as [Hugging Face](https://huggingface.co/), [Torch Vision](https://pytorch.org/vision/stable/index.html), and [ONNX Model Zoo](https://github.com/onnx/models#models), by leveraging zero-code optimization solution [Neural Coder](/neural_coder#what-do-we-offer) and automatic [accuracy-driven](/docs/source/design.md#workflow) quantization strategies
 
 * Collaborate with cloud marketplaces such as [Google Cloud Platform](https://console.cloud.google.com/marketplace/product/bitnami-launchpad/inc-tensorflow-intel?project=verdant-sensor-286207), [Amazon Web Services](https://aws.amazon.com/marketplace/pp/prodview-yjyh2xmggbmga#pdp-support), and [Azure](https://azuremarketplace.microsoft.com/en-us/marketplace/apps/bitnami.inc-tensorflow-intel), software platforms such as [Alibaba Cloud](https://www.intel.com/content/www/us/en/developer/articles/technical/quantize-ai-by-oneapi-analytics-on-alibaba-cloud.html), [Tencent TACO](https://new.qq.com/rain/a/20221202A00B9S00) and [Microsoft Olive](https://github.com/microsoft/Olive), and open AI ecosystem such as [Hugging Face](https://huggingface.co/blog/intel), [PyTorch](https://pytorch.org/tutorials/recipes/intel_neural_compressor_for_pytorch.html), [ONNX](https://github.com/onnx/models#models), [ONNX Runtime](https://github.com/microsoft/onnxruntime), and [Lightning AI](https://github.com/Lightning-AI/lightning/blob/master/docs/source-pytorch/advanced/post_training_quantization.rst)
 
+## What's New
+* [2024/03] A new SOTA approach [AutoRound](https://github.com/intel/auto-round) Weight-Only Quantization on [Intel Gaudi2 AI accelerator](https://habana.ai/products/gaudi2/) is available for LLMs.
+
 ## Installation
 
 ### Install from pypi
 ```Shell
 pip install neural-compressor
 ```
 > **Note**: 
 > More installation methods can be found at [Installation Guide](https://github.com/intel/neural-compressor/blob/master/docs/source/installation_guide.md). Please check out our [FAQ](https://github.com/intel/neural-compressor/blob/master/docs/source/faq.md) for more details.
 
 ## Getting Started
-### Quantization with Python API
 
-```shell
-# Install Intel Neural Compressor and TensorFlow
-pip install neural-compressor
-pip install tensorflow
-# Prepare fp32 model
-wget https://storage.googleapis.com/intel-optimized-tensorflow/models/v1_6/mobilenet_v1_1.0_224_frozen.pb
+Setting up the environment:  
+```bash
+pip install "neural-compressor>=2.3" "transformers>=4.34.0" torch torchvision
 ```
+After successfully installing these packages, try your first quantization program.
+
+### Weight-Only Quantization (LLMs)
+Following example code demonstrates Weight-Only Quantization on LLMs, it supports Intel CPU, Intel Gauid2 AI Accelerator, Nvidia GPU, best device will be selected automatically. 
+
+To try on Intel Gaudi2, docker image with Gaudi Software Stack is recommended, please refer to following script for environment setup. More details can be found in [Gaudi Guide](https://docs.habana.ai/en/latest/Installation_Guide/Bare_Metal_Fresh_OS.html#launch-docker-image-that-was-built). 
+```bash
+docker run -it --runtime=habana -e HABANA_VISIBLE_DEVICES=all -e OMPI_MCA_btl_vader_single_copy_mechanism=none --cap-add=sys_nice --net=host --ipc=host vault.habana.ai/gaudi-docker/1.14.0/ubuntu22.04//habanalabs/pytorch-installer-2.1.1:latest
+
+# Check the container ID
+docker ps
+
+# Login into container
+docker exec -it <container_id> bash
+
+# Install the optimum-habana
+pip install --upgrade-strategy eager optimum[habana]
+
+# Install INC/auto_round
+pip install neural-compressor auto_round
+```
+Run the example:
 ```python
-from neural_compressor.data import DataLoader, Datasets
+from transformers import AutoModel, AutoTokenizer
+
 from neural_compressor.config import PostTrainingQuantConfig
+from neural_compressor.quantization import fit
+from neural_compressor.adaptor.torch_utils.auto_round import get_dataloader
+
+model_name = "EleutherAI/gpt-neo-125m"
+float_model = AutoModel.from_pretrained(model_name)
+tokenizer = AutoTokenizer.from_pretrained(model_name, trust_remote_code=True)
+dataloader = get_dataloader(tokenizer, seqlen=2048)
+
+woq_conf = PostTrainingQuantConfig(
+    approach="weight_only",
+    op_type_dict={
+        ".*": {  # match all ops
+            "weight": {
+                "dtype": "int",
+                "bits": 4,
+                "algorithm": "AUTOROUND",
+            },
+        }
+    },
+)
+quantized_model = fit(model=float_model, conf=woq_conf, calib_dataloader=dataloader)
+```
+**Note:** 
+
+To try INT4 model inference, please directly use [Intel Extension for Transformers](https://github.com/intel/intel-extension-for-transformers), which leverages Intel Neural Compressor for model quantization.        
 
-dataset = Datasets("tensorflow")["dummy"](shape=(1, 224, 224, 3))
-dataloader = DataLoader(framework="tensorflow", dataset=dataset)
+### Static Quantization (Non-LLMs)
 
+```python
+from torchvision import models
+
+from neural_compressor.config import PostTrainingQuantConfig
+from neural_compressor.data import DataLoader, Datasets
 from neural_compressor.quantization import fit
 
-q_model = fit(
-    model="./mobilenet_v1_1.0_224_frozen.pb",
-    conf=PostTrainingQuantConfig(),
-    calib_dataloader=dataloader,
-)
+float_model = models.resnet18()
+dataset = Datasets("pytorch")["dummy"](shape=(1, 3, 224, 224))
+calib_dataloader = DataLoader(framework="pytorch", dataset=dataset)
+static_quant_conf = PostTrainingQuantConfig()
+quantized_model = fit(model=float_model, conf=static_quant_conf, calib_dataloader=calib_dataloader)
 ```
 
 ## Documentation
 
 <table class="docutils">
   <thead>
   <tr>
     <th colspan="8">Overview</th>
   </tr>
   </thead>
   <tbody>
     <tr>
       <td colspan="2" align="center"><a href="./docs/source/design.md#architecture">Architecture</a></td>
       <td colspan="2" align="center"><a href="./docs/source/design.md#workflow">Workflow</a></td>
+      <td colspan="1" align="center"><a href="https://intel.github.io/neural-compressor/latest/docs/source/api-doc/apis.html">APIs</a></td>
+      <td colspan="1" align="center"><a href="./docs/source/llm_recipes.md">LLMs Recipes</a></td>
       <td colspan="2" align="center"><a href="examples/README.md">Examples</a></td>
-      <td colspan="2" align="center"><a href="https://intel.github.io/neural-compressor/latest/docs/source/api-doc/apis.html">APIs</a></td>
     </tr>
   </tbody>
   <thead>
     <tr>
       <th colspan="8">Python-based APIs</th>
     </tr>
   </thead>
```

### Comparing `neural_solution-2.4/neural_solution.egg-info/SOURCES.txt` & `neural_solution-2.5.1/neural_solution.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neural_solution-2.4/pyproject.toml` & `neural_solution-2.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `neural_solution-2.4/third-party-programs.txt` & `neural_solution-2.5.1/third-party-programs.txt`

 * *Files 0% similar despite different names*

```diff
@@ -70,14 +70,16 @@
    Diffusers
 
    web-vitals
    Copyright 2020 Google LLC
 
    web-worker
 
+   segment-anything
+
 
                                 Apache License
                             Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

