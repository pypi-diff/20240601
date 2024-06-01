# Comparing `tmp/paka-0.1.8.tar.gz` & `tmp/paka-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paka-0.1.8.tar", max compression
+gzip compressed data, was "paka-0.1.9.tar", max compression
```

## Comparing `paka-0.1.8.tar` & `paka-0.1.9.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0     1072 2024-05-19 08:14:16.473163 paka-0.1.8/LICENSE
--rw-r--r--   0        0        0     4321 2024-05-19 08:14:16.473163 paka-0.1.8/README.md
--rw-r--r--   0        0        0      153 2024-05-19 08:14:16.477163 paka-0.1.8/paka/__init__.py
--rw-r--r--   0        0        0        0 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cli/__init__.py
--rw-r--r--   0        0        0     1608 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cli/__main__.py
--rw-r--r--   0        0        0     1402 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cli/build.py
--rw-r--r--   0        0        0     4449 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cli/cluster.py
--rw-r--r--   0        0        0    14006 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cli/function.py
--rw-r--r--   0        0        0     5666 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cli/job.py
--rw-r--r--   0        0        0      903 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cli/kubeconfig.py
--rw-r--r--   0        0        0     2577 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cli/model_group.py
--rw-r--r--   0        0        0     3443 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cli/run.py
--rw-r--r--   0        0        0    11534 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cli/utils.py
--rw-r--r--   0        0        0        0 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/__init__.py
--rw-r--r--   0        0        0        0 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/aws/__init__.py
--rw-r--r--   0        0        0      968 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/aws/cloudwatch.py
--rw-r--r--   0        0        0     3982 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/aws/cluster_autoscaler.py
--rw-r--r--   0        0        0      542 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/aws/container_registry.py
--rw-r--r--   0        0        0     2466 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/aws/ebs_csi_driver.py
--rw-r--r--   0        0        0    15960 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/aws/eks.py
--rw-r--r--   0        0        0     1732 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/aws/elb.py
--rw-r--r--   0        0        0      569 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/aws/object_store.py
--rw-r--r--   0        0        0     3969 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/aws/service_account.py
--rw-r--r--   0        0        0     1904 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/aws/utils.py
--rw-r--r--   0        0        0     4136 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/context.py
--rw-r--r--   0        0        0     4580 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/fluentbit.py
--rw-r--r--   0        0        0     1189 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/keda.py
--rw-r--r--   0        0        0     4981 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/knative.py
--rw-r--r--   0        0        0     2480 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/kubectl.py
--rw-r--r--   0        0        0        0 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/manager/__init__.py
--rw-r--r--   0        0        0      928 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/manager/aws.py
--rw-r--r--   0        0        0     3485 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/manager/base.py
--rw-r--r--   0        0        0      914 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/namespace.py
--rw-r--r--   0        0        0     3484 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/nvidia_device_plugin.py
--rw-r--r--   0        0        0     4275 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/prometheus.py
--rw-r--r--   0        0        0     3600 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/pulumi.py
--rw-r--r--   0        0        0     3998 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/qdrant.py
--rw-r--r--   0        0        0     2286 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/redis.py
--rw-r--r--   0        0        0      284 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/utils.py
--rw-r--r--   0        0        0      908 2024-05-19 08:14:16.477163 paka-0.1.8/paka/cluster/zipkin.py
--rw-r--r--   0        0        0    22175 2024-05-19 08:14:16.477163 paka-0.1.8/paka/config.py
--rw-r--r--   0        0        0      467 2024-05-19 08:14:16.477163 paka-0.1.8/paka/constants.py
--rw-r--r--   0        0        0     3623 2024-05-19 08:14:16.477163 paka-0.1.8/paka/container/ecr.py
--rw-r--r--   0        0        0     2627 2024-05-19 08:14:16.477163 paka-0.1.8/paka/container/pack.py
--rw-r--r--   0        0        0     6536 2024-05-19 08:14:16.477163 paka-0.1.8/paka/gguf.py
--rw-r--r--   0        0        0        0 2024-05-19 08:14:16.477163 paka-0.1.8/paka/k8s/function/__init__.py
--rw-r--r--   0        0        0    11603 2024-05-19 08:14:16.477163 paka-0.1.8/paka/k8s/function/service.py
--rw-r--r--   0        0        0        0 2024-05-19 08:14:16.477163 paka-0.1.8/paka/k8s/job/__init__.py
--rw-r--r--   0        0        0     2370 2024-05-19 08:14:16.477163 paka-0.1.8/paka/k8s/job/autoscaler.py
--rw-r--r--   0        0        0     4093 2024-05-19 08:14:16.477163 paka-0.1.8/paka/k8s/job/worker.py
--rw-r--r--   0        0        0        0 2024-05-19 08:14:16.477163 paka-0.1.8/paka/k8s/model_group/__init__.py
--rw-r--r--   0        0        0     1364 2024-05-19 08:14:16.477163 paka-0.1.8/paka/k8s/model_group/ingress.py
--rw-r--r--   0        0        0      131 2024-05-19 08:14:16.477163 paka-0.1.8/paka/k8s/model_group/manifest.py
--rw-r--r--   0        0        0        0 2024-05-19 08:14:16.477163 paka-0.1.8/paka/k8s/model_group/runtime/__init__.py
--rw-r--r--   0        0        0     4820 2024-05-19 08:14:16.477163 paka-0.1.8/paka/k8s/model_group/runtime/llama_cpp.py
--rw-r--r--   0        0        0     1883 2024-05-19 08:14:16.477163 paka-0.1.8/paka/k8s/model_group/runtime/vllm.py
--rw-r--r--   0        0        0    22683 2024-05-19 08:14:16.477163 paka-0.1.8/paka/k8s/model_group/service.py
--rw-r--r--   0        0        0     9948 2024-05-19 08:14:16.477163 paka-0.1.8/paka/k8s/model_group/service_v1.py
--rw-r--r--   0        0        0    21190 2024-05-19 08:14:16.477163 paka-0.1.8/paka/k8s/utils.py
--rw-r--r--   0        0        0      761 2024-05-19 08:14:16.477163 paka-0.1.8/paka/logger.py
--rw-r--r--   0        0        0        0 2024-05-19 08:14:16.477163 paka-0.1.8/paka/model/__init__.py
--rw-r--r--   0        0        0     2705 2024-05-19 08:14:16.477163 paka-0.1.8/paka/model/base_model.py
--rw-r--r--   0        0        0     2462 2024-05-19 08:14:16.477163 paka-0.1.8/paka/model/hf_model.py
--rw-r--r--   0        0        0     1488 2024-05-19 08:14:16.477163 paka-0.1.8/paka/model/http_model.py
--rw-r--r--   0        0        0     1444 2024-05-19 08:14:16.477163 paka-0.1.8/paka/model/manifest.py
--rw-r--r--   0        0        0     2565 2024-05-19 08:14:16.477163 paka-0.1.8/paka/model/progress_bar.py
--rw-r--r--   0        0        0     2080 2024-05-19 08:14:16.477163 paka-0.1.8/paka/model/settings.py
--rw-r--r--   0        0        0    10006 2024-05-19 08:14:16.477163 paka-0.1.8/paka/model/store.py
--rw-r--r--   0        0        0    12339 2024-05-19 08:14:16.477163 paka-0.1.8/paka/utils.py
--rw-r--r--   0        0        0     1630 2024-05-19 08:14:16.481163 paka-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     5728 1970-01-01 00:00:00.000000 paka-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-06-01 18:06:23.739436 paka-0.1.9/LICENSE
+-rw-r--r--   0        0        0     5092 2024-06-01 18:06:23.739436 paka-0.1.9/README.md
+-rw-r--r--   0        0        0      153 2024-06-01 18:06:23.747436 paka-0.1.9/paka/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-01 18:06:23.747436 paka-0.1.9/paka/cli/__init__.py
+-rw-r--r--   0        0        0     1608 2024-06-01 18:06:23.747436 paka-0.1.9/paka/cli/__main__.py
+-rw-r--r--   0        0        0     2186 2024-06-01 18:06:23.747436 paka-0.1.9/paka/cli/build.py
+-rw-r--r--   0        0        0     4449 2024-06-01 18:06:23.747436 paka-0.1.9/paka/cli/cluster.py
+-rw-r--r--   0        0        0    14161 2024-06-01 18:06:23.747436 paka-0.1.9/paka/cli/function.py
+-rw-r--r--   0        0        0     6704 2024-06-01 18:06:23.747436 paka-0.1.9/paka/cli/job.py
+-rw-r--r--   0        0        0      903 2024-06-01 18:06:23.747436 paka-0.1.9/paka/cli/kubeconfig.py
+-rw-r--r--   0        0        0     3303 2024-06-01 18:06:23.747436 paka-0.1.9/paka/cli/model_group.py
+-rw-r--r--   0        0        0     3443 2024-06-01 18:06:23.747436 paka-0.1.9/paka/cli/run.py
+-rw-r--r--   0        0        0    11774 2024-06-01 18:06:23.747436 paka-0.1.9/paka/cli/utils.py
+-rw-r--r--   0        0        0        0 2024-06-01 18:06:23.747436 paka-0.1.9/paka/cluster/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-01 18:06:23.747436 paka-0.1.9/paka/cluster/aws/__init__.py
+-rw-r--r--   0        0        0      968 2024-06-01 18:06:23.747436 paka-0.1.9/paka/cluster/aws/cloudwatch.py
+-rw-r--r--   0        0        0     3982 2024-06-01 18:06:23.747436 paka-0.1.9/paka/cluster/aws/cluster_autoscaler.py
+-rw-r--r--   0        0        0      542 2024-06-01 18:06:23.747436 paka-0.1.9/paka/cluster/aws/container_registry.py
+-rw-r--r--   0        0        0     2466 2024-06-01 18:06:23.747436 paka-0.1.9/paka/cluster/aws/ebs_csi_driver.py
+-rw-r--r--   0        0        0    18436 2024-06-01 18:06:23.747436 paka-0.1.9/paka/cluster/aws/eks.py
+-rw-r--r--   0        0        0     1732 2024-06-01 18:06:23.747436 paka-0.1.9/paka/cluster/aws/elb.py
+-rw-r--r--   0        0        0      569 2024-06-01 18:06:23.747436 paka-0.1.9/paka/cluster/aws/object_store.py
+-rw-r--r--   0        0        0     3969 2024-06-01 18:06:23.747436 paka-0.1.9/paka/cluster/aws/service_account.py
+-rw-r--r--   0        0        0     2915 2024-06-01 18:06:23.747436 paka-0.1.9/paka/cluster/aws/utils.py
+-rw-r--r--   0        0        0     4136 2024-06-01 18:06:23.747436 paka-0.1.9/paka/cluster/context.py
+-rw-r--r--   0        0        0     4580 2024-06-01 18:06:23.747436 paka-0.1.9/paka/cluster/fluentbit.py
+-rw-r--r--   0        0        0     1189 2024-06-01 18:06:23.747436 paka-0.1.9/paka/cluster/keda.py
+-rw-r--r--   0        0        0     4981 2024-06-01 18:06:23.747436 paka-0.1.9/paka/cluster/knative.py
+-rw-r--r--   0        0        0     2480 2024-06-01 18:06:23.747436 paka-0.1.9/paka/cluster/kubectl.py
+-rw-r--r--   0        0        0        0 2024-06-01 18:06:23.747436 paka-0.1.9/paka/cluster/manager/__init__.py
+-rw-r--r--   0        0        0      928 2024-06-01 18:06:23.747436 paka-0.1.9/paka/cluster/manager/aws.py
+-rw-r--r--   0        0        0     3485 2024-06-01 18:06:23.747436 paka-0.1.9/paka/cluster/manager/base.py
+-rw-r--r--   0        0        0      914 2024-06-01 18:06:23.747436 paka-0.1.9/paka/cluster/namespace.py
+-rw-r--r--   0        0        0     3484 2024-06-01 18:06:23.747436 paka-0.1.9/paka/cluster/nvidia_device_plugin.py
+-rw-r--r--   0        0        0     4262 2024-06-01 18:06:23.747436 paka-0.1.9/paka/cluster/prometheus.py
+-rw-r--r--   0        0        0     3600 2024-06-01 18:06:23.747436 paka-0.1.9/paka/cluster/pulumi.py
+-rw-r--r--   0        0        0     3997 2024-06-01 18:06:23.747436 paka-0.1.9/paka/cluster/qdrant.py
+-rw-r--r--   0        0        0     2284 2024-06-01 18:06:23.747436 paka-0.1.9/paka/cluster/redis.py
+-rw-r--r--   0        0        0      284 2024-06-01 18:06:23.747436 paka-0.1.9/paka/cluster/utils.py
+-rw-r--r--   0        0        0      908 2024-06-01 18:06:23.747436 paka-0.1.9/paka/cluster/zipkin.py
+-rw-r--r--   0        0        0    23858 2024-06-01 18:06:23.747436 paka-0.1.9/paka/config.py
+-rw-r--r--   0        0        0      467 2024-06-01 18:06:23.747436 paka-0.1.9/paka/constants.py
+-rw-r--r--   0        0        0     3793 2024-06-01 18:06:23.747436 paka-0.1.9/paka/container/ecr.py
+-rw-r--r--   0        0        0     2627 2024-06-01 18:06:23.747436 paka-0.1.9/paka/container/pack.py
+-rw-r--r--   0        0        0     6536 2024-06-01 18:06:23.747436 paka-0.1.9/paka/gguf.py
+-rw-r--r--   0        0        0        0 2024-06-01 18:06:23.747436 paka-0.1.9/paka/k8s/function/__init__.py
+-rw-r--r--   0        0        0    14236 2024-06-01 18:06:23.747436 paka-0.1.9/paka/k8s/function/service.py
+-rw-r--r--   0        0        0        0 2024-06-01 18:06:23.747436 paka-0.1.9/paka/k8s/job/__init__.py
+-rw-r--r--   0        0        0     2370 2024-06-01 18:06:23.747436 paka-0.1.9/paka/k8s/job/autoscaler.py
+-rw-r--r--   0        0        0     6242 2024-06-01 18:06:23.747436 paka-0.1.9/paka/k8s/job/worker.py
+-rw-r--r--   0        0        0        0 2024-06-01 18:06:23.747436 paka-0.1.9/paka/k8s/model_group/__init__.py
+-rw-r--r--   0        0        0     1364 2024-06-01 18:06:23.747436 paka-0.1.9/paka/k8s/model_group/ingress.py
+-rw-r--r--   0        0        0      131 2024-06-01 18:06:23.747436 paka-0.1.9/paka/k8s/model_group/manifest.py
+-rw-r--r--   0        0        0        0 2024-06-01 18:06:23.747436 paka-0.1.9/paka/k8s/model_group/runtime/__init__.py
+-rw-r--r--   0        0        0     4820 2024-06-01 18:06:23.747436 paka-0.1.9/paka/k8s/model_group/runtime/llama_cpp.py
+-rw-r--r--   0        0        0     1944 2024-06-01 18:06:23.747436 paka-0.1.9/paka/k8s/model_group/runtime/vllm.py
+-rw-r--r--   0        0        0    24410 2024-06-01 18:06:23.747436 paka-0.1.9/paka/k8s/model_group/service.py
+-rw-r--r--   0        0        0     9948 2024-06-01 18:06:23.747436 paka-0.1.9/paka/k8s/model_group/service_v1.py
+-rw-r--r--   0        0        0    21190 2024-06-01 18:06:23.747436 paka-0.1.9/paka/k8s/utils.py
+-rw-r--r--   0        0        0      761 2024-06-01 18:06:23.747436 paka-0.1.9/paka/logger.py
+-rw-r--r--   0        0        0        0 2024-06-01 18:06:23.747436 paka-0.1.9/paka/model/__init__.py
+-rw-r--r--   0        0        0     2705 2024-06-01 18:06:23.747436 paka-0.1.9/paka/model/base_model.py
+-rw-r--r--   0        0        0     2462 2024-06-01 18:06:23.751436 paka-0.1.9/paka/model/hf_model.py
+-rw-r--r--   0        0        0     1488 2024-06-01 18:06:23.751436 paka-0.1.9/paka/model/http_model.py
+-rw-r--r--   0        0        0     1444 2024-06-01 18:06:23.751436 paka-0.1.9/paka/model/manifest.py
+-rw-r--r--   0        0        0     2565 2024-06-01 18:06:23.751436 paka-0.1.9/paka/model/progress_bar.py
+-rw-r--r--   0        0        0     2080 2024-06-01 18:06:23.751436 paka-0.1.9/paka/model/settings.py
+-rw-r--r--   0        0        0    10006 2024-06-01 18:06:23.751436 paka-0.1.9/paka/model/store.py
+-rw-r--r--   0        0        0    12727 2024-06-01 18:06:23.751436 paka-0.1.9/paka/utils.py
+-rw-r--r--   0        0        0     1630 2024-06-01 18:06:23.751436 paka-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     6499 1970-01-01 00:00:00.000000 paka-0.1.9/PKG-INFO
```

### Comparing `paka-0.1.8/LICENSE` & `paka-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `paka-0.1.8/paka/cli/__main__.py` & `paka-0.1.9/paka/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.8/paka/cli/build.py` & `paka-0.1.9/paka/cli/build.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from __future__ import annotations
 
 import os
 from typing import Optional
 
 import typer
 
-from paka.cli.utils import build_and_push
+from paka.cli.utils import build_and_push, ensure_cluster_name, push_to_ecr
+from paka.utils import read_pulumi_stack
 
 build_app = typer.Typer()
 
 
-@build_app.callback(invoke_without_command=True)
-def build(
+@build_app.command()
+def build_image(
     cluster_name: Optional[str] = typer.Option(
         os.getenv("PAKA_CURRENT_CLUSTER"),
         "--cluster",
         "-c",
         help="The name of the cluster.",
     ),
     source_dir: str = typer.Argument(
@@ -37,7 +38,34 @@
     files and directories to exclude from the image. Once the image is built,
     it will be pushed to the container repository of the current cluster.
 
     A Dockerfile is NOT required. The image will be built using Cloud Native Buildpacks.
     In cluster build is not supported yet. User machine must have Docker installed.
     """
     build_and_push(cluster_name, source_dir, image_name)
+
+
+@build_app.command()
+def push_image(
+    cluster_name: Optional[str] = typer.Option(
+        os.getenv("PAKA_CURRENT_CLUSTER"),
+        "--cluster",
+        "-c",
+        help="The name of the cluster.",
+    ),
+    image_name: str = typer.Option(
+        "",
+        "--image-name",
+        help="Name of the pre-built Docker image. If image tag is not provided, 'latest' will be used.",
+    ),
+) -> None:
+    """
+    Push a pre-built Docker image to the container repository of the current cluster.
+    """
+    cluster_name = ensure_cluster_name(cluster_name)
+
+    push_to_ecr(
+        image_name,
+        read_pulumi_stack(cluster_name, "registry"),
+        read_pulumi_stack(cluster_name, "region"),
+        image_name,
+    )
```

### Comparing `paka-0.1.8/paka/cli/cluster.py` & `paka-0.1.9/paka/cli/cluster.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.8/paka/cli/function.py` & `paka-0.1.9/paka/cli/function.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from kubernetes.client.exceptions import ApiException
 from tabulate import tabulate
 
 from paka.cli.utils import (
     format_timedelta,
     get_cluster_namespace,
     load_kubeconfig,
+    process_envs,
     resolve_image,
 )
 from paka.k8s.function.service import (
     create_knative_service,
     delete_knative_service,
     list_knative_revisions,
     list_knative_services,
@@ -112,19 +113,18 @@
         None,
         "--image",
         help="The name of the Docker image to deploy. If both an image and a "
         "source directory are provided, this image will be used and the source "
         "directory will be ignored.",
     ),
     min_instances: int = typer.Option(
-        0,
+        1,
         "--min-replicas",
         help="The minimum number of instances to be maintained at all times to "
-        "handle incoming requests. The default value is 0, indicating that the "
-        "system can scale down to zero instances when no requests are being processed.",
+        "handle incoming requests. The default value is 0.",
     ),
     max_instances: int = typer.Option(
         0,
         "--max-replicas",
         help="The maximum number of instances that can be created to handle peak "
         "load. The default value is set to 0, indicating that there is no upper "
         "limit on the number of instances that can be created.",
@@ -134,26 +134,32 @@
         "--scaling-metric",
         help="The performance metric that the scaling system should monitor to "
         "determine when to adjust the number of instances.",
         case_sensitive=True,
         click_type=click.Choice(["rps", "concurrency"]),
     ),
     metric_target: int = typer.Option(
-        10,
+        1,
         "--metric-target",
         help="The desired value for the chosen scaling metric. The system will "
         "adjust the number of active instances to attempt to reach this target.",
     ),
     scale_down_delay: str = typer.Option(
         "0s",
         "--scale-down-delay",
         help="The delay before the system scales down after a spike in traffic. "
         "This value must be a duration between 0 seconds and 1 hour, represented "
         "as a string (e.g., '0s', '1m', '1h').",
     ),
+    env_vars: List[str] = typer.Option(
+        [],
+        "--env",
+        help="Specify environment variables for the function in the format 'key=value'",
+        show_default=False,
+    ),
     resource_requests: Optional[str] = typer.Option(
         None,
         "--resource-requests",
         help='The resource requests for the function, in JSON format. For example: \'{"cpu": "100m", "memory": "128Mi"}\'',
     ),
     resource_limits: Optional[str] = typer.Option(
         None,
@@ -170,23 +176,26 @@
     logger.info(f"Deploying {name}...")
 
     resource_requests_dict = (
         json.loads(resource_requests) if resource_requests else None
     )
     resource_limits_dict = json.loads(resource_limits) if resource_limits else None
 
+    envs = process_envs(env_vars)
+
     create_knative_service(
         service_name=kubify_name(name),
         namespace=get_cluster_namespace(cluster_name),
         image=resolved_image,
         entrypoint=entrypoint,
         min_instances=min_instances,
         max_instances=max_instances,
         scaling_metric=(scaling_metric, str(metric_target)),
         scale_down_delay=scale_down_delay,
+        envs=envs,
         resource_requests=resource_requests_dict,
         resource_limits=resource_limits_dict,
     )
 
     logger.info(f"Successfully deployed {name}")
```

### Comparing `paka-0.1.8/paka/cli/job.py` & `paka-0.1.9/paka/cli/job.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 from __future__ import annotations
 
+import json
 import os
-from typing import Optional
+from typing import List, Optional
 
 import typer
 from kubernetes import client
 
-from paka.cli.utils import get_cluster_namespace, load_kubeconfig, resolve_image
+from paka.cli.utils import (
+    get_cluster_namespace,
+    load_kubeconfig,
+    process_envs,
+    resolve_image,
+)
 from paka.k8s.job.worker import create_workers, delete_workers
 from paka.logger import logger
 from paka.utils import kubify_name
 
 job_app = typer.Typer()
 
 
@@ -76,34 +82,59 @@
     wait_existing_tasks: bool = typer.Option(
         True,
         "--wait-existing-tasks",
         help="Determines whether the system should wait for existing tasks to "
         "complete before deploying the new job. If set to true, the deployment "
         "will wait until all current tasks have finished.",
     ),
+    env_vars: List[str] = typer.Option(
+        [],
+        "--env",
+        help="Specify environment variables for the function in the format 'key=value'",
+        show_default=False,
+    ),
+    resource_requests: Optional[str] = typer.Option(
+        None,
+        "--resource-requests",
+        help='The resource requests for the function, in JSON format. For example: \'{"cpu": "100m", "memory": "128Mi"}\'',
+    ),
+    resource_limits: Optional[str] = typer.Option(
+        None,
+        "--resource-limits",
+        help='The resource limits for the function, in JSON format. For example: \'{"cpu": "200m", "memory": "256Mi"}\'',
+    ),
 ) -> None:
     """
     Deploy a job.
     """
     load_kubeconfig(cluster_name)
     resolved_image = resolve_image(cluster_name, image, source_dir)
 
     if image:
         job_name = image
     elif source_dir:
         job_name = os.path.basename(source_dir)
 
+    envs = process_envs(env_vars)
+    resource_requests_dict = (
+        json.loads(resource_requests) if resource_requests else None
+    )
+    resource_limits_dict = json.loads(resource_limits) if resource_limits else None
+
     create_workers(
         namespace=get_cluster_namespace(cluster_name),
         job_name=kubify_name(prefixed_job_name(name or job_name)),
         image=resolved_image,
         entrypoint=entrypoint,
         tasks_per_worker=tasks_per_worker,
         max_replicas=max_workers,
         drain_existing_job=wait_existing_tasks,
+        envs=envs,
+        resource_requests=resource_requests_dict,
+        resource_limits=resource_limits_dict,
     )
 
 
 @job_app.command()
 def delete(
     cluster_name: Optional[str] = typer.Option(
         os.getenv("PAKA_CURRENT_CLUSTER"),
```

### Comparing `paka-0.1.8/paka/cli/kubeconfig.py` & `paka-0.1.9/paka/cli/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.8/paka/cli/model_group.py` & `paka-0.1.9/paka/cli/model_group.py`

 * *Files 17% similar despite different names*

```diff
@@ -64,27 +64,49 @@
     ),
 ) -> None:
     """
     List all model groups.
     """
     load_kubeconfig(cluster_name)
     services = filter_services(get_cluster_namespace(cluster_name))
-    model_groups = [
+
+    # Get public model groups
+    public_model_groups = [
+        service.spec.selector.get("model", "")
+        for service in services
+        if service.spec
+        and service.spec.selector
+        and "model" in service.spec.selector
+        and service.metadata
+        and service.metadata.labels
+        and (service.metadata.labels.get("is-public", "false") == "true")
+    ]
+
+    # Get private model groups
+    private_model_groups = [
         service.spec.selector.get("model", "")
         for service in services
-        if service.spec and service.spec.selector and "model" in service.spec.selector
+        if service.spec
+        and service.spec.selector
+        and "model" in service.spec.selector
+        and service.metadata
+        and service.metadata.labels
+        and (service.metadata.labels.get("is-public", "false") == "false")
     ]
 
+    model_groups = public_model_groups + private_model_groups
+
     v1 = client.CoreV1Api()
     cfg = v1.read_namespaced_config_map("config-domain", "knative-serving")
     cfg_data = cfg.data or {}
     filtered_keys = [key for key in cfg_data if key.endswith("sslip.io")]
     if not filtered_keys:
         if not model_groups:
             logger.info("No model groups found.")
         else:
             logger.info("\n".join(model_groups))
         return
     domain = filtered_keys[0]
 
-    table = [(group, f"http://{group}.{domain}") for group in model_groups]
+    table = [(group, f"http://{group}.{domain}") for group in public_model_groups]
+    table.extend([(group, f"private") for group in private_model_groups])
     logger.info(tabulate(table, headers=["Model Group", "Endpoint"]))
```

### Comparing `paka-0.1.8/paka/cli/run.py` & `paka-0.1.9/paka/cli/run.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.8/paka/cli/utils.py` & `paka-0.1.9/paka/cli/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import functools
 import os
 import platform
 import re
 import subprocess
 from datetime import timedelta
-from typing import Any, Optional
+from typing import Any, Dict, List, Optional
 
 import typer
 from kubernetes import config as k8s_config
 
 from paka.cluster.manager.aws import AWSClusterManager
 from paka.cluster.manager.base import ClusterManager
 from paka.config import CloudConfig, Config, parse_yaml
@@ -321,7 +321,16 @@
         return f"{days}d{hours}h"
     elif hours > 0:
         return f"{hours}h{minutes}m"
     elif minutes > 0:
         return f"{minutes}m{seconds}s"
     else:
         return f"{seconds}s"
+
+
+def process_envs(envs: List[str]) -> Dict[str, str]:
+    env_dict = {}
+    for env in envs:
+        for pair in env.split(","):
+            key, value = pair.split("=", 1)
+            env_dict[key] = value
+    return env_dict
```

### Comparing `paka-0.1.8/paka/cluster/aws/cloudwatch.py` & `paka-0.1.9/paka/cluster/aws/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.8/paka/cluster/aws/cluster_autoscaler.py` & `paka-0.1.9/paka/cluster/aws/cluster_autoscaler.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.8/paka/cluster/aws/container_registry.py` & `paka-0.1.9/paka/cluster/aws/container_registry.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.8/paka/cluster/aws/ebs_csi_driver.py` & `paka-0.1.9/paka/cluster/aws/ebs_csi_driver.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.8/paka/cluster/aws/eks.py` & `paka-0.1.9/paka/cluster/aws/eks.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,24 +10,25 @@
 import pulumi_kubernetes as k8s
 
 from paka.cluster.aws.cloudwatch import enable_cloudwatch
 from paka.cluster.aws.cluster_autoscaler import create_cluster_autoscaler
 from paka.cluster.aws.ebs_csi_driver import create_ebs_csi_driver
 from paka.cluster.aws.elb import update_elb_idle_timeout
 from paka.cluster.aws.service_account import create_service_accounts
+from paka.cluster.aws.utils import create_vpc_endpoint_for_s3, get_ami_for_instance
 from paka.cluster.context import Context
 from paka.cluster.keda import create_keda
 from paka.cluster.knative import create_knative_and_istio
 from paka.cluster.namespace import create_namespace
 from paka.cluster.nvidia_device_plugin import install_nvidia_device_plugin
 from paka.cluster.prometheus import create_prometheus
 from paka.cluster.qdrant import create_qdrant
 from paka.cluster.redis import create_redis
 from paka.cluster.zipkin import create_zipkin
-from paka.config import AwsMixedModelGroup, AwsModelGroup
+from paka.config import AwsMixedModelGroup, AwsModelGroup, NodeGroup
 from paka.k8s.utils import update_kubeconfig
 from paka.utils import kubify_name
 
 
 def _ignore_tags_transformation(
     args: pulumi.ResourceTransformationArgs,
 ) -> Optional[pulumi.ResourceTransformationResult]:
@@ -86,22 +87,18 @@
                 effect="NO_SCHEDULE", key="app", value="model-group"
             ),
             aws.eks.NodeGroupTaintArgs(
                 effect="NO_SCHEDULE", key="model", value=model_group.name
             ),
         ]
 
-        gpu_enabled = model_group.gpu and model_group.gpu.enabled
-
-        ami_type = "AL2_x86_64_GPU" if gpu_enabled else None
+        ami_type = get_ami_for_instance(ctx, model_group.nodeType)
 
         disk_size = (
-            model_group.gpu.diskSize
-            if gpu_enabled and model_group.gpu
-            else model_group.diskSize
+            model_group.gpu.diskSize if model_group.gpu else model_group.diskSize
         )
 
         # Create a managed node group for our cluster
         eks.ManagedNodeGroup(
             f"{cluster_name}-{kubify_name(model_group.name)}-group",
             node_group_name=f"{cluster_name}-{kubify_name(model_group.name)}-on-demand",
             cluster=cluster,
@@ -149,21 +146,19 @@
                 effect="NO_SCHEDULE", key="app", value="model-group"
             ),
             aws.eks.NodeGroupTaintArgs(
                 effect="NO_SCHEDULE", key="model", value=mixed_model_group.name
             ),
         ]
 
-        gpu_enabled = mixed_model_group.gpu and mixed_model_group.gpu.enabled
-
-        ami_type = "AL2_x86_64_GPU" if gpu_enabled else None
+        ami_type = get_ami_for_instance(ctx, mixed_model_group.nodeType)
 
         disk_size = (
             mixed_model_group.gpu.diskSize
-            if gpu_enabled and mixed_model_group.gpu
+            if mixed_model_group.gpu
             else mixed_model_group.diskSize
         )
 
         # Create a managed node group for our cluster
         eks.ManagedNodeGroup(
             f"{cluster_name}-{kubify_name(mixed_model_group.name)}-group",
             node_group_name=f"{cluster_name}-{kubify_name(mixed_model_group.name)}-on-demand",
@@ -269,14 +264,91 @@
             "app": "qdrant",
         },
         node_role_arn=worker_role.arn,
         subnet_ids=vpc.private_subnet_ids,
         taints=[
             aws.eks.NodeGroupTaintArgs(effect="NO_SCHEDULE", key="app", value="qdrant"),
         ],
+        disk_size=vectorStore.diskSize,
+    )
+
+
+def _create_node_groups(
+    ctx: Context,
+    cluster: eks.Cluster,
+    vpc: awsx.ec2.Vpc,
+    worker_role: aws.iam.Role,
+    app: str,
+    node_groups: Optional[List[NodeGroup]],
+) -> None:
+    if node_groups is None:
+        return
+
+    cluster_name = ctx.cluster_name
+    for i, node_group in enumerate(node_groups):
+        ami_type = get_ami_for_instance(ctx, node_group.nodeTypes[0])
+
+        lifecycle = node_group.isSpot and "spot" or "on-demand"
+        # Create a managed node group for our cluster
+        eks.ManagedNodeGroup(
+            f"{cluster_name}-{app}-group-{i}",
+            node_group_name=f"{cluster_name}-{app}-group-{i}-{lifecycle}",
+            cluster=cluster,
+            instance_types=node_group.nodeTypes,
+            scaling_config=aws.eks.NodeGroupScalingConfigArgs(
+                desired_size=node_group.minInstances,
+                min_size=node_group.minInstances,
+                max_size=node_group.maxInstances,
+            ),
+            labels={
+                "app": app,
+                "lifecycle": lifecycle,
+            },
+            node_role_arn=worker_role.arn,
+            subnet_ids=vpc.private_subnet_ids,
+            taints=[
+                aws.eks.NodeGroupTaintArgs(effect="NO_SCHEDULE", key="app", value=app),
+            ],
+            disk_size=node_group.diskSize,
+            capacity_type="SPOT" if node_group.isSpot else "ON_DEMAND",
+            ami_type=ami_type,
+        )
+
+
+def create_node_groups_for_functions(
+    ctx: Context,
+    cluster: eks.Cluster,
+    vpc: awsx.ec2.Vpc,
+    worker_role: aws.iam.Role,
+) -> None:
+    """
+    Creates a managed node group for functions
+    """
+    if ctx.cloud_config.function is None:
+        return
+
+    _create_node_groups(
+        ctx, cluster, vpc, worker_role, "function", ctx.cloud_config.function.nodeGroups
+    )
+
+
+def create_node_groups_for_job(
+    ctx: Context,
+    cluster: eks.Cluster,
+    vpc: awsx.ec2.Vpc,
+    worker_role: aws.iam.Role,
+) -> None:
+    """
+    Creates a managed node group for functions
+    """
+    if ctx.cloud_config.job is None:
+        return
+
+    _create_node_groups(
+        ctx, cluster, vpc, worker_role, "job", ctx.cloud_config.job.nodeGroups
     )
 
 
 def create_k8s_cluster(ctx: Context) -> eks.Cluster:
     """
     Provisions an AWS EKS cluster with the necessary resources.
 
@@ -336,14 +408,19 @@
                 "type": awsx.ec2.SubnetType.PRIVATE,
                 "tags": {"kubernetes.io/role/internal-elb": "1"},
             },
         ],
         opts=pulumi.ResourceOptions(transformations=[_ignore_tags_transformation]),
     )
 
+    route_table_ids = vpc.route_tables.apply(
+        lambda route_tables: [rt.id for rt in route_tables]
+    )
+    create_vpc_endpoint_for_s3(vpc.vpc_id, route_table_ids, ctx.region)
+
     cluster = eks.Cluster(
         cluster_name,
         vpc_id=vpc.vpc_id,
         public_subnet_ids=vpc.public_subnet_ids,
         private_subnet_ids=vpc.private_subnet_ids,
         node_associate_public_ip_address=False,
         create_oidc_provider=True,
@@ -372,14 +449,17 @@
     create_node_group_for_model_group(ctx, cluster, vpc, worker_role)
 
     create_node_group_for_mixed_model_group(ctx, cluster, vpc, worker_role)
 
     # Create a managed node group for Qdrant
     create_node_group_for_qdrant(ctx, cluster, vpc, worker_role)
 
+    create_node_groups_for_functions(ctx, cluster, vpc, worker_role)
+    create_node_groups_for_job(ctx, cluster, vpc, worker_role)
+
     def create_eks_resources(kubeconfig_json: str) -> None:
         k8s_provider = k8s.Provider("k8s-provider", kubeconfig=cluster.kubeconfig)
         ctx.set_k8s_provider(k8s_provider)
         ctx.set_kubeconfig(kubeconfig_json)
 
         if ctx.should_save_kubeconfig:
             update_kubeconfig(json.loads(kubeconfig_json))
```

### Comparing `paka-0.1.8/paka/cluster/aws/elb.py` & `paka-0.1.9/paka/cluster/aws/elb.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.8/paka/cluster/aws/object_store.py` & `paka-0.1.9/paka/cluster/aws/object_store.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.8/paka/cluster/aws/service_account.py` & `paka-0.1.9/paka/cluster/aws/service_account.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.8/paka/cluster/context.py` & `paka-0.1.9/paka/cluster/context.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.8/paka/cluster/fluentbit.py` & `paka-0.1.9/paka/cluster/fluentbit.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.8/paka/cluster/keda.py` & `paka-0.1.9/paka/cluster/keda.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.8/paka/cluster/knative.py` & `paka-0.1.9/paka/cluster/knative.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.8/paka/cluster/kubectl.py` & `paka-0.1.9/paka/cluster/kubectl.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.8/paka/cluster/manager/aws.py` & `paka-0.1.9/paka/cluster/manager/aws.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.8/paka/cluster/manager/base.py` & `paka-0.1.9/paka/cluster/manager/base.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.8/paka/cluster/namespace.py` & `paka-0.1.9/paka/cluster/namespace.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.8/paka/cluster/nvidia_device_plugin.py` & `paka-0.1.9/paka/cluster/nvidia_device_plugin.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.8/paka/cluster/prometheus.py` & `paka-0.1.9/paka/cluster/prometheus.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,55 +35,55 @@
         opts=pulumi.ResourceOptions(provider=ctx.k8s_provider),
     )
 
     return Chart(
         "kube-prometheus-stack",
         ChartOpts(
             chart="kube-prometheus-stack",
-            version="56.3.0",
+            version="58.6.0",
             namespace="prometheus",
             fetch_opts=FetchOpts(
                 repo="https://prometheus-community.github.io/helm-charts"
             ),
             values={
                 "nodeExporter": {
-                    "enabled": config.prometheus.node_exporter,
+                    "enabled": config.prometheus.nodeExporter,
                 },
                 "alertmanager": {
                     "enabled": config.prometheus.alertmanager,
                 },
                 "grafana": {
                     "enabled": config.prometheus.grafana,
                 },
                 "kubeApiServer": {
-                    "enabled": config.prometheus.kube_api_server,
+                    "enabled": config.prometheus.kubeApiServer,
                 },
                 "kubelet": {
                     "enabled": config.prometheus.kubelet,
                 },
                 "kubeControllerManager": {
-                    "enabled": config.prometheus.kube_controller_manager,
+                    "enabled": config.prometheus.kubeControllerManager,
                 },
                 "coreDns": {
-                    "enabled": config.prometheus.core_dns,
+                    "enabled": config.prometheus.coreDns,
                 },
                 "kubeEtcd": {
-                    "enabled": config.prometheus.kube_etcd,
+                    "enabled": config.prometheus.kubeEtcd,
                 },
                 "kubeScheduler": {
-                    "enabled": config.prometheus.kube_scheduler,
+                    "enabled": config.prometheus.kubeScheduler,
                 },
                 "kubeProxy": {
-                    "enabled": config.prometheus.kube_proxy,
+                    "enabled": config.prometheus.kubeProxy,
                 },
                 "kubeStateMetrics": {
-                    "enabled": config.prometheus.kube_state_metrics,
+                    "enabled": config.prometheus.kubeStateMetrics,
                 },
                 "thanosRuler": {
-                    "enabled": config.prometheus.thanos_ruler,
+                    "enabled": config.prometheus.thanosRuler,
                 },
                 # Disable the Prometheus Operator's admission webhooks, since they don't work with Pulumi.
                 # This means ill-formatted Prometheus rules may make their way into Prometheus. :(
                 "prometheusOperator": {
                     "admissionWebhooks": {"enabled": False},
                     "tls": {"enabled": False},
                 },
@@ -99,15 +99,15 @@
                         "podMonitorSelectorNilUsesHelmValues": False,
                         "storageSpec": {
                             "volumeClaimTemplate": {
                                 "spec": {
                                     "accessModes": ["ReadWriteOnce"],
                                     "resources": {
                                         "requests": {
-                                            "storage": config.prometheus.storage_size,
+                                            "storage": config.prometheus.storageSize,
                                         }
                                     },
                                 }
                             }
                         },
                     }
                 },
```

### Comparing `paka-0.1.8/paka/cluster/pulumi.py` & `paka-0.1.9/paka/cluster/pulumi.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.8/paka/cluster/qdrant.py` & `paka-0.1.9/paka/cluster/qdrant.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
                             if config.prometheus and config.prometheus.enabled
                             else False
                         ),
                     },
                 },
                 "replicaCount": config.vectorStore.replicas,
                 "persistence": {
-                    "size": config.vectorStore.storage_size,
+                    "size": config.vectorStore.storageSize,
                 },
                 "livenessProbe": {
                     "enabled": True,
                 },
                 "tolerations": [
                     {
                         "key": "app",
```

### Comparing `paka-0.1.8/paka/cluster/redis.py` & `paka-0.1.9/paka/cluster/redis.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             namespace=ctx.namespace,
             fetch_opts=FetchOpts(repo="https://charts.bitnami.com/bitnami"),
             values={
                 "architecture": "standalone",
                 "master": {
                     "persistence": {
                         "enabled": True,
-                        "size": config.job.broker_storage_size,
+                        "size": config.job.brokerStorageSize,
                     },
                 },
                 "metrics": {"enabled": True},  # For enabling metrics
             },
         ),
         opts=pulumi.ResourceOptions(provider=ctx.k8s_provider, depends_on=[ns]),
     )
```

### Comparing `paka-0.1.8/paka/cluster/zipkin.py` & `paka-0.1.9/paka/cluster/zipkin.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.8/paka/config.py` & `paka-0.1.9/paka/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Any, Dict, Generic, List, Optional, TypeVar
 
 from pydantic import BaseModel, ConfigDict, Field, field_validator, model_validator
 from ruamel.yaml import YAML
 
 from paka.utils import to_yaml
 
-CONFIG_VERSION = "1.1"
+CONFIG_VERSION = "1.3"
 
 
 class PakaBaseModel(BaseModel):
     model_config = ConfigDict(extra="forbid")
 
 
 def validate_size(v: str, error_message: str = "Invalid size format") -> str:
@@ -153,14 +153,18 @@
     Represents a runtime for a model.
     """
 
     image: str = Field(..., description="The Docker image to use for the runtime.")
     command: Optional[List[str]] = Field(
         None, description="The command to run in the Docker container."
     )
+    env: Optional[List[Dict[str, Any]]] = None
+    readinessProbe: Optional[Dict[str, Any]] = None
+    livenessProbe: Optional[Dict[str, Any]] = None
+    volumeMounts: Optional[List[Dict[str, Any]]] = None
 
 
 class Model(PakaBaseModel):
     """
     Represents a model.
     """
 
@@ -268,20 +272,41 @@
 
         Returns:
             int: The input value if validation is successful.
 
         Raises:
             ValueError: If the value of the input value is invalid.
         """
+        if v < 0:
+            raise ValueError("minInstances cannot be negative")
+        return v
+
+
+class ScalingConfigNonZero(ScalingConfig):
+    @field_validator("minInstances", mode="before")
+    def validate_min_instances(cls, v: int) -> int:
+        """
+        Validates the value of the minInstances field. Spinning up 1 model group instance is heavy.
+        No scaling down to 0 for now.
+
+        Args:
+            v (int): The value of the minInstances field.
+
+        Returns:
+            int: The input value if validation is successful.
+
+        Raises:
+            ValueError: If the value of the input value is invalid.
+        """
         if v <= 0:
             raise ValueError("minInstances must be greater than 0")
         return v
 
 
-class OnDemandModelGroup(CloudModelGroup, ScalingConfig):
+class OnDemandModelGroup(CloudModelGroup, ScalingConfigNonZero):
     pass
 
 
 class MixedModelGroup(CloudModelGroup):
     baseInstances: int = Field(
         ...,
         description=(
@@ -295,15 +320,15 @@
         description=(
             "This sets the maximum limit for provisioning on-demand instances, including the base instances. "
             "It should always be set to a value equal to or greater than 'baseInstances'. "
             "These on-demand instances serve as a fallback when spot instances are unavailable. "
             "The actual number of on-demand instances is dynamically adjusted by the autoscaler based on the workload requirements."
         ),
     )
-    spot: ScalingConfig = Field(
+    spot: ScalingConfigNonZero = Field(
         ...,
         description=(
             "This configuration sets the scaling parameters for spot instances within the node group. "
             "It specifies the minimum and maximum number of spot instances that can be used. "
             "Spot instances are cost-effective but may not always be available due to market conditions. "
             "The autoscaler uses this configuration to dynamically adjust the number of spot instances based on workload demand."
         ),
@@ -363,37 +388,37 @@
 
 class CloudVectorStore(CloudNode):
     """
     Represents a cloud vector store.
     """
 
     replicas: int = Field(1, description="The number of replicas for the vector store.")
-    storage_size: str = Field(
+    storageSize: str = Field(
         "10Gi", description="The size of the storage of one node for the vector store."
     )
     resourceRequest: Optional[ResourceRequest] = Field(
         None,
         description="The resource request for the vector store, specifying the amount of CPU and memory to request.",
     )
 
-    @field_validator("storage_size", mode="before")
+    @field_validator("storageSize", mode="before")
     def validate_storage_size(cls, v: str) -> str:
         """
         Validates the format of the storage_size field.
 
         Args:
             v (str): The value of the storage_size field.
 
         Returns:
             str: The input value if validation is successful.
 
         Raises:
             ValueError: If the format of the input value is invalid.
         """
-        return validate_size(v, "Invalid storage size format")
+        return validate_size(v, "Invalid size format")
 
     @field_validator("replicas", mode="before")
     def validate_replicas(cls, v: int) -> int:
         """
         Validates the value of the replicas field.
 
         Args:
@@ -406,94 +431,116 @@
             ValueError: If the value of the input value is invalid.
         """
         if v <= 0:
             raise ValueError("replicas must be greater than 0")
         return v
 
 
+class NodeGroup(ScalingConfigNonZero):
+    nodeTypes: List[str] = Field(
+        ..., description="The types of nodes in the node group."
+    )
+    diskSize: Optional[int] = Field(
+        None, description="The size of the disk for the node in GB."
+    )
+    isSpot: bool = Field(..., description="Whether the node group uses spot instances.")
+
+
 class Job(PakaBaseModel):
     """
     Represents a job cluster configuration.
     """
 
     enabled: bool = Field(False, description="Whether the job cluster is enabled.")
-    broker_storage_size: str = Field(
+    brokerStorageSize: str = Field(
         "10Gi", description="The size of the storage for the broker."
     )
 
-    @field_validator("broker_storage_size", mode="before")
+    nodeGroups: Optional[List[NodeGroup]] = Field(
+        None,
+        description="The node groups for job workers. If None, default node groups are used.",
+    )
+
+    @field_validator("brokerStorageSize", mode="before")
     def validate_broker_storage_size(cls, v: str) -> str:
         """
-        Validates the format of the broker_storage_size field.
+        Validates the format of the brokerStorageSize field.
 
         Args:
-            v (str): The value of the storage_size field.
+            v (str): The value of the brokerStorageSize field.
 
         Returns:
             str: The input value if validation is successful.
 
         Raises:
             ValueError: If the format of the input value is invalid.
         """
-        return validate_size(v, "Invalid storage size format")
+        return validate_size(v, "Invalid size format")
+
+
+class Function(PakaBaseModel):
+    """
+    Configuration for function.
+    """
+
+    nodeGroups: Optional[List[NodeGroup]] = Field(
+        None,
+        description="The node groups for functions. If None, default node groups are used.",
+    )
 
 
 class Prometheus(PakaBaseModel):
     """
     Represents a Prometheus configuration.
     """
 
     enabled: bool = Field(False, description="Whether Prometheus is enabled.")
-    storage_size: str = Field(
+    storageSize: str = Field(
         "10Gi", description="The size of the storage for Prometheus."
     )
     grafana: bool = Field(False, description="Whether Grafana is enabled.")
     alertmanager: bool = Field(False, description="Whether Alertmanager is enabled.")
-    kube_api_server: bool = Field(
+    kubeApiServer: bool = Field(
         False, description="Whether the Kubernetes API server is enabled."
     )
     kubelet: bool = Field(False, description="Whether the Kubelet is enabled.")
-    kube_controller_manager: bool = Field(
+    kubeControllerManager: bool = Field(
         False, description="Whether the Kubernetes controller manager is enabled."
     )
-    core_dns: bool = Field(False, description="Whether CoreDNS is enabled.")
-    kube_etcd: bool = Field(
-        False, description="Whether the Kubernetes etcd is enabled."
-    )
-    kube_scheduler: bool = Field(
+    coreDns: bool = Field(False, description="Whether CoreDNS is enabled.")
+    kubeEtcd: bool = Field(False, description="Whether the Kubernetes etcd is enabled.")
+    kubeScheduler: bool = Field(
         False, description="Whether the Kubernetes scheduler is enabled."
     )
-    kube_proxy: bool = Field(
+    kubeProxy: bool = Field(
         False, description="Whether the Kubernetes proxy is enabled."
     )
-    kube_state_metrics: bool = Field(
+    kubeStateMetrics: bool = Field(
         False, description="Whether the Kubernetes state metrics are enabled."
     )
-    node_exporter: bool = Field(
+    nodeExporter: bool = Field(
         False, description="Whether the Node Exporter is enabled."
     )
-    thanos_ruler: bool = Field(
-        False, description="Whether the Thanos Ruler is enabled."
-    )
+    thanosRuler: bool = Field(False, description="Whether the Thanos Ruler is enabled.")
 
-    @field_validator("storage_size", mode="before")
+    @field_validator("storageSize", mode="before")
     def validate_storage_size(cls, v: str) -> str:
         """
-        Validates the format of the storage_size field.
+        Validates the format of the storageSize field.
 
         Args:
-            v (str): The value of the storage_size field.
+            v (str): The value of the storageSize field.
 
         Returns:
             str: The input value if validation is successful.
 
         Raises:
             ValueError: If the format of the input value is invalid.
         """
-        return validate_size(v, "Invalid storage size format")
+        return validate_size(v, "Invalid size format")
 
 
 class Tracing(PakaBaseModel):
     """
     Represents the configuration for tracing.
     """
 
@@ -527,14 +574,17 @@
         None,
         description="The list of mixed model groups to be deployed in the cloud. Default is None. If None, no mixed model groups are deployed.",
     )
     vectorStore: Optional[CloudVectorStore] = Field(
         None,
         description="The configuration for the vector store in the cloud. Default is None. If None, no vector store is deployed",
     )
+    function: Optional[Function] = Field(
+        None, description="The configuration for functions. Default is None."
+    )
     job: Optional[Job] = Field(
         None,
         description="The configuration for the job broker. Default is None. If None, no job broker is deployed.",
     )
     prometheus: Optional[Prometheus] = Field(
         None,
         description="The configuration for Prometheus. Default is None. If None, Prometheus is not deployed.",
```

### Comparing `paka-0.1.8/paka/container/ecr.py` & `paka-0.1.9/paka/container/ecr.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,30 +31,30 @@
         return ecr_url
     except Exception as e:
         print(f"An error occurred: {str(e)}")
         raise
 
 
 def push_to_ecr(
-    image_name: str, repository_uri: str, aws_region: str, app_name: str
+    local_image_name: str, repository_uri: str, aws_region: str, app_name: str
 ) -> str:
     """
     Pushes a Docker image to an Amazon ECR repository.
 
     This function tags the Docker image with a version tag and the "latest" tag,
     logs in to the ECR repository, and pushes the image to the repository.
     The version tag is generated randomly.
 
     All applications share the same container registry repository.
     To differentiate between them, we append the application name to the image tag.
     The '-latest' suffix is added to handle cases where applications themselves are tagged.
     This ensures that even tagged applications have a unique identifier in the shared repository.
 
     Args:
-        image_name (str): The name of the Docker image to push.
+        local_image_name (str): The name of the Docker image to push.
         repository_uri (str): The URI of the ECR repository to push the image to.
         aws_region (str): The AWS region where the ECR repository is located.
         app_name (str): The name of the application. Used to generate the image tags.
 
     Raises:
         subprocess.CalledProcessError: If an error occurs while executing a subprocess command.
 
@@ -64,44 +64,50 @@
     try:
         # Generate a random version number
         version = random_str()
 
         # Tag the image with the repository URI and the version tag
         version_tag = f"{app_name}-v{version}"
 
+        local_image_tagged = (
+            f"{local_image_name}:latest"
+            if ":" not in local_image_name
+            else local_image_name
+        )
+
         # Tag the image with the repository URI
         subprocess.run(
             [
                 "docker",
                 "tag",
-                f"{image_name}:latest",
+                local_image_tagged,
                 f"{repository_uri}:{version_tag}",
             ],
             check=True,
         )
 
         # Tag the image with the repository URI and the "latest" tag
         latest_tag = f"{app_name}-latest"
         subprocess.run(
             [
                 "docker",
                 "tag",
-                f"{image_name}:latest",
+                local_image_tagged,
                 f"{repository_uri}:{latest_tag}",
             ],
             check=True,
         )
 
         # Authenticate Docker to the ECR
         authenticate_docker_to_ecr(aws_region)
 
         # Push the image to the ECR repository
         subprocess.run(
             ["docker", "push", f"{repository_uri}:{version_tag}"], check=True
         )
         subprocess.run(["docker", "push", f"{repository_uri}:{latest_tag}"], check=True)
 
-        logger.info(f"Successfully pushed {image_name} to {repository_uri}")
+        logger.info(f"Successfully pushed {local_image_name} to {repository_uri}")
         return version_tag
     except subprocess.CalledProcessError as e:
         logger.error(f"An error occurred: {e}")
         raise
```

### Comparing `paka-0.1.8/paka/container/pack.py` & `paka-0.1.9/paka/container/pack.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.8/paka/gguf.py` & `paka-0.1.9/paka/gguf.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.8/paka/k8s/function/service.py` & `paka-0.1.9/paka/k8s/function/service.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import shlex
 from typing import Any, Dict, List, Literal, Optional, Tuple
 
 from kubernetes import client
 from kubernetes.client.exceptions import ApiException
 from kubernetes.dynamic import DynamicClient  # type: ignore
 
+from paka.k8s.utils import apply_resource
+
 VALID_RESOURCES = ["cpu", "memory"]
 
 VALID_RESOURCES_GPU = ["nvidia.com/gpu"]
 
 
 def validate_resource(resource: str, value: str) -> None:
     if resource == "cpu":
@@ -56,17 +58,18 @@
     entrypoint: str,
     min_instances: int,
     max_instances: int,
     # concurrency refers to the number of simultaneous requests that a single pod can handle
     # rps refers to requests per second a single pod can handle
     scaling_metric: Tuple[Literal["concurrency", "rps"], str],
     scale_down_delay: str = "0s",
+    envs: Optional[Dict[str, str]] = None,
     resource_requests: Optional[Dict[str, str]] = None,
     resource_limits: Optional[Dict[str, str]] = None,
-) -> None:
+) -> Dict[str, Any]:
     """
     Creates a Knative Service with the specified configuration.
 
     This function creates a Knative Service with the provided service name, namespace, image,
     minimum and maximum instances, scaling metric, and scale down delay.
 
     The function validates the input parameters and raises a ValueError if any of them are invalid.
@@ -86,28 +89,51 @@
         ValueError: If any of the input parameters are invalid.
 
     Returns:
         None
     """
     if not isinstance(min_instances, int) or not isinstance(max_instances, int):
         raise ValueError("min_replicas and max_replicas must be integers")
-    if min_instances > max_instances:
+    if min_instances > max_instances and not max_instances == 0:
         raise ValueError("min_replicas cannot be greater than max_replicas")
 
     metric_key, metric_value = scaling_metric
     if metric_key not in ["concurrency", "rps"]:
         raise ValueError(f"Invalid key in scaling_metric: {metric_key}")
     if not metric_value.isdigit():
         raise ValueError(f"Invalid value in scaling_metric: {metric_value}")
 
+    config_map = client.V1ConfigMap(
+        kind="ConfigMap",
+        metadata=client.V1ObjectMeta(
+            name="config-features", namespace="knative-serving"
+        ),
+        data={
+            "kubernetes.podspec-tolerations": "enabled",
+            "kubernetes.podspec-affinity": "enabled",
+        },
+    )
+
+    apply_resource(config_map)
+
     container: Dict[str, Any] = {
         "image": image,
         "imagePullPolicy": "Always",
         "command": shlex.split(entrypoint),
     }
+    if envs:
+        container["env"] = [
+            {"name": key, "value": value} for key, value in envs.items()
+        ]
+
+    # Set a default value for resources if not provided
+    container["resources"] = {
+        "requests": {"cpu": "100m", "memory": "128Mi"},
+        "limits": {"cpu": "200m", "memory": "256Mi"},
+    }
 
     if resource_limits or resource_requests:
         container["resources"] = {}
 
     if resource_requests:
         if not all(key in VALID_RESOURCES for key in resource_requests.keys()):
             raise ValueError(
@@ -149,15 +175,55 @@
                         "autoscaling.knative.dev/class": "kpa.autoscaling.knative.dev",
                         "autoscaling.knative.dev/min-scale": str(min_instances),
                         "autoscaling.knative.dev/max-scale": str(max_instances),
                         "autoscaling.knative.dev/scale-down-delay": scale_down_delay,
                         **metric,
                     },
                 },
-                "spec": {"containers": [container]},
+                "spec": {
+                    "containers": [container],
+                    "tolerations": [
+                        {
+                            "key": "app",
+                            "operator": "Equal",
+                            "value": "function",
+                            "effect": "NoSchedule",
+                        }
+                    ],
+                    "affinity": {
+                        "nodeAffinity": {
+                            "preferredDuringSchedulingIgnoredDuringExecution": [
+                                {
+                                    "weight": 100,
+                                    "preference": {
+                                        "matchExpressions": [
+                                            {
+                                                "key": "lifecycle",
+                                                "operator": "In",
+                                                "values": ["spot"],
+                                            }
+                                        ]
+                                    },
+                                },
+                                {
+                                    "weight": 50,
+                                    "preference": {
+                                        "matchExpressions": [
+                                            {
+                                                "key": "lifecycle",
+                                                "operator": "In",
+                                                "values": ["on-demand"],
+                                            }
+                                        ]
+                                    },
+                                },
+                            ]
+                        },
+                    },
+                },
             }
         },
     }
 
     k8s_client = client.ApiClient()
     dyn_client = DynamicClient(k8s_client)
 
@@ -174,14 +240,15 @@
             content_type="application/merge-patch+json",
         )
     except ApiException as e:
         if e.status == 404:
             service_resource.create(body=knative_service, namespace=namespace)
         else:
             raise
+    return knative_service
 
 
 def list_knative_services(namespace: str) -> Any:
     """
     List all Knative Services in the specified namespace.
 
     Args:
```

### Comparing `paka-0.1.8/paka/k8s/job/autoscaler.py` & `paka-0.1.9/paka/k8s/job/autoscaler.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.8/paka/k8s/model_group/ingress.py` & `paka-0.1.9/paka/k8s/model_group/ingress.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.8/paka/k8s/model_group/runtime/llama_cpp.py` & `paka-0.1.9/paka/k8s/model_group/runtime/llama_cpp.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.8/paka/k8s/model_group/runtime/vllm.py` & `paka-0.1.9/paka/k8s/model_group/runtime/vllm.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,17 @@
 
     def attach_model_to_command(command: List[str]) -> List[str]:
         return command + ["--model", model_to_load]
 
     if runtime.command:
         return attach_model_to_command(runtime.command)
 
-    command = shlex.split("python3 -O -u -m vllm.entrypoints.api_server --host 0.0.0.0")
+    command = shlex.split(
+        f"python3 -O -u -m vllm.entrypoints.openai.api_server --host 0.0.0.0 --served-model-name {model_group.name}"
+    )
 
     gpu_count = get_gpu_count(ctx, model_group)
 
     if gpu_count > 1:
         command += ["--tensor-parallel-size", str(gpu_count)]
 
     return attach_model_to_command(command)
```

### Comparing `paka-0.1.8/paka/k8s/model_group/service.py` & `paka-0.1.9/paka/k8s/model_group/service.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import json
-from typing import List, Optional, Tuple, cast
+from typing import Any, Dict, List, Optional, Tuple, Union, cast
 
 from kubernetes import client
 from kubernetes import config as k8s_config
 
 from paka.cluster.context import Context
 from paka.cluster.utils import get_model_store
 from paka.config import CloudModelGroup, T_OnDemandModelGroup
@@ -16,15 +16,15 @@
     is_llama_cpp_image,
 )
 from paka.k8s.model_group.runtime.vllm import get_runtime_command_vllm, is_vllm_image
 from paka.k8s.utils import CustomResource, apply_resource, get_gpu_count
 from paka.logger import logger
 from paka.model.hf_model import HuggingFaceModel
 from paka.model.store import MODEL_PATH_PREFIX
-from paka.utils import get_instance_info, kubify_name
+from paka.utils import camel_to_snake, get_instance_info, kubify_name
 
 
 def get_runtime_command(
     ctx: Context, model_group: CloudModelGroup, port: int
 ) -> List[str]:
     """
     Gets the runtime command for a machine learning model group.
@@ -63,14 +63,87 @@
         return ("/health", "/health")
     elif is_vllm_image(model_group.runtime.image):
         return ("/health", "/health")
 
     raise ValueError("Unsupported runtime image for health check paths.")
 
 
+def create_volume_mounts(
+    volumeMounts: Optional[List[Dict[str, Any]]]
+) -> List[client.V1VolumeMount]:
+    default_volume_mount = [
+        client.V1VolumeMount(name="model-data", mount_path=MODEL_MOUNT_PATH)
+    ]
+
+    if volumeMounts:
+        volume_mounts = [
+            client.V1VolumeMount(
+                name=vm["name"], mount_path=vm["mountPath"], sub_path=vm.get("subPath")
+            )
+            for vm in volumeMounts
+        ]
+
+        if any(vm.name == "model-data" for vm in volume_mounts):
+            return volume_mounts
+        else:
+            return default_volume_mount + volume_mounts
+    return default_volume_mount
+
+
+def create_env_vars(
+    env: Optional[List[Dict[str, Any]]], port: int
+) -> List[client.V1EnvVar]:
+    if not env:
+        return [client.V1EnvVar(name="PORT", value=str(port))]
+
+    env_vars = [client.V1EnvVar(name=var["name"], value=var["value"]) for var in env]
+
+    # Replace the PORT env var if it exists
+    for var in env_vars:
+        if var.name == "PORT":
+            var.value = str(port)
+
+    # If PORT env var does not exist, add it
+    if not any(var.name == "PORT" for var in env_vars):
+        env_vars.append(client.V1EnvVar(name="PORT", value=str(port)))
+
+    return env_vars
+
+
+def create_probe(
+    pod_spec_probe: Optional[Union[client.V1Probe, Dict[str, Any]]],
+    path: str,
+    port: int,
+    initial_delay_seconds: int,
+) -> client.V1Probe:
+    if pod_spec_probe:
+        if isinstance(pod_spec_probe, dict):
+            http_get = client.V1HTTPGetAction(
+                **{
+                    camel_to_snake(k): v
+                    for k, v in pod_spec_probe.pop("httpGet").items()
+                }
+            )
+            return client.V1Probe(
+                http_get=http_get,
+                **{camel_to_snake(k): v for k, v in pod_spec_probe.items()},
+            )
+        return pod_spec_probe
+
+    # Return a default probe
+    return client.V1Probe(
+        http_get=client.V1HTTPGetAction(path=path, port=port),
+        initial_delay_seconds=initial_delay_seconds,
+        period_seconds=5,
+        timeout_seconds=30,
+        success_threshold=1,
+        failure_threshold=5,
+    )
+
+
 def init_aws(ctx: Context, model_group: CloudModelGroup) -> client.V1Container:
     """
     Initializes an AWS container for downloading a model from S3.
 
     Args:
         config (CloudConfig): The cloud configuration.
         model_group (T_CloudModelGroup): The cloud model group.
@@ -124,100 +197,79 @@
         ValueError: If the AWS configuration is not provided.
 
     Returns:
         client.V1Pod: The created Pod.
     """
     ready_probe_path, live_probe_path = get_health_check_paths(model_group)
 
+    env, volume_mounts, readiness_probe, liveness_probe = (
+        model_group.runtime.env,
+        model_group.runtime.volumeMounts,
+        model_group.runtime.readinessProbe,
+        model_group.runtime.livenessProbe,
+    )
+
     container_args = {
         "name": f"{kubify_name(model_group.name)}",
         "image": model_group.runtime.image,
         "command": get_runtime_command(ctx, model_group, port),
-        "volume_mounts": [
-            client.V1VolumeMount(
-                name="model-data",
-                mount_path=MODEL_MOUNT_PATH,
-            )
-        ],
-        "env": [
-            client.V1EnvVar(
-                name="PORT",
-                value=str(port),
-            ),
-        ],
+        "volume_mounts": create_volume_mounts(volume_mounts),
+        "env": create_env_vars(env, port),
         "ports": [client.V1ContainerPort(container_port=port)],
-        "readiness_probe": client.V1Probe(
-            http_get=client.V1HTTPGetAction(
-                path=ready_probe_path,
-                port=port,
-            ),
-            initial_delay_seconds=60,
-            period_seconds=5,
-            timeout_seconds=30,
-            success_threshold=1,
-            failure_threshold=5,
+        "readiness_probe": create_probe(
+            readiness_probe if readiness_probe else None, ready_probe_path, port, 60
         ),
-        "liveness_probe": client.V1Probe(
-            http_get=client.V1HTTPGetAction(
-                path=live_probe_path,
-                port=port,
-            ),
-            initial_delay_seconds=240,
-            period_seconds=30,
-            timeout_seconds=30,
-            success_threshold=1,
-            failure_threshold=5,
+        "liveness_probe": create_probe(
+            liveness_probe if liveness_probe else None, live_probe_path, port, 240
         ),
     }
 
     if model_group.resourceRequest:
         cpu_request = model_group.resourceRequest.cpu
         memory_request = model_group.resourceRequest.memory
     else:
-        instance_info = get_instance_info(
-            ctx.provider, ctx.region, model_group.nodeType
-        )
-        if not instance_info:
-            raise ValueError(
-                f"No instance information found for instance type {model_group.nodeType} in {ctx.provider} {ctx.region}"
-            )
-        cpu_milli = cast(int, instance_info["cpu"]) * 1000
-        # Leave 400m for other processes
-        cpu_request = f"{cpu_milli - 400}m"
-        # Leave 2GB for other processes
-        memory_request = f"{cast(int, instance_info['memory']) - (2 * 1024)}Mi"
+        # Set low resource requests to guarantee that the pod is scheduled.
+        # This is fine as the pod will be able to use up to the node limit.
+        cpu_request = f"1000m"
+        memory_request = f"1024Mi"
 
     resources = client.V1ResourceRequirements(
         requests={
             "cpu": cpu_request,
             "memory": memory_request,
         },
     )
 
     container_args["resources"] = resources
 
+    enable_host_ipc = False
+
     if hasattr(model_group, "gpu") and model_group.gpu and model_group.gpu.enabled:
         if resources.limits is None:
             resources.limits = {}
 
         gpu_count = get_gpu_count(ctx=ctx, model_group=model_group)
 
         # Ah, we only support nvidia GPUs for now
         resources.limits["nvidia.com/gpu"] = str(gpu_count)
 
+        if gpu_count > 1 and is_vllm_image(model_group.runtime.image):
+            enable_host_ipc = True
+
     return client.V1PodTemplateSpec(
         metadata=client.V1ObjectMeta(
             name=f"{kubify_name(model_group.name)}",
             namespace=namespace,
             labels={
                 "app": "model-group",
                 "model": model_group.name,
             },
         ),
         spec=client.V1PodSpec(
+            host_ipc=enable_host_ipc,
             service_account_name=ACCESS_ALL_SA,
             volumes=[
                 client.V1Volume(
                     name="model-data",
                     empty_dir=client.V1EmptyDirVolumeSource(),
                 )
             ],
@@ -338,15 +390,15 @@
 
     # Both llama-cpp and vllm servers expose metrics on /metrics
     if is_llama_cpp_image(model_group.runtime.image) or is_vllm_image(
         model_group.runtime.image
     ):
         monitor.spec["endpoints"].append(
             {
-                "port": "http",
+                "port": "http-app",
                 "path": "/metrics",
                 "interval": "15s",
             }
         )
     apply_resource(monitor)
 
 
@@ -374,14 +426,15 @@
         kind="Service",
         metadata=client.V1ObjectMeta(
             name=f"{kubify_name(model_group.name)}",
             namespace=namespace,
             labels={
                 "app": "model-group",
                 "model": model_group.name,
+                "is-public": "true" if model_group.isPublic else "false",
             },
         ),
         spec=client.V1ServiceSpec(
             selector={
                 "app": "model-group",
                 "model": model_group.name,
             },
```

### Comparing `paka-0.1.8/paka/k8s/model_group/service_v1.py` & `paka-0.1.9/paka/k8s/model_group/service_v1.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.8/paka/k8s/utils.py` & `paka-0.1.9/paka/k8s/utils.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.8/paka/logger.py` & `paka-0.1.9/paka/logger.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.8/paka/model/base_model.py` & `paka-0.1.9/paka/model/base_model.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.8/paka/model/hf_model.py` & `paka-0.1.9/paka/model/hf_model.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.8/paka/model/http_model.py` & `paka-0.1.9/paka/model/http_model.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.8/paka/model/manifest.py` & `paka-0.1.9/paka/model/manifest.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.8/paka/model/progress_bar.py` & `paka-0.1.9/paka/model/progress_bar.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.8/paka/model/settings.py` & `paka-0.1.9/paka/model/settings.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.8/paka/model/store.py` & `paka-0.1.9/paka/model/store.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.8/paka/utils.py` & `paka-0.1.9/paka/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,30 +19,30 @@
 from ruamel.yaml import YAML
 
 from paka.constants import HOME_ENV_VAR, PROJECT_NAME, PULUMI_STACK_NAME
 
 T = TypeVar("T", bound=Callable[..., Any])
 
 
-def camel_to_kebab(name: str) -> str:
+def camel_to_kebab(camel_str: str) -> str:
     """
     Converts a camel case string to kebab case.
 
     Args:
-        name (str): The camel case string to be converted.
+        camel_str (str): The camel case string to be converted.
 
     Returns:
         str: The kebab case string.
 
     Example:
         >>> camel_to_kebab("camelCaseString")
         'camel-case-string'
     """
-    name = re.sub("(.)([A-Z][a-z]+)", r"\1-\2", name)
-    return re.sub("([a-z0-9])([A-Z])", r"\1-\2", name).lower()
+    camel_str = re.sub("(.)([A-Z][a-z]+)", r"\1-\2", camel_str)
+    return re.sub("([a-z0-9])([A-Z])", r"\1-\2", camel_str).lower()
 
 
 def kubify_name(old: str) -> str:
     """
     Convert a string into a valid Kubernetes name.
 
     This function takes a string, converts it to lowercase, replaces disallowed characters with '-',
@@ -386,20 +386,30 @@
         response = ec2.describe_instance_types(InstanceTypes=[instance_type])  # type: ignore
 
         instance_types = response.get("InstanceTypes", [])
         if instance_types:
             instance_type_info = instance_types[0]
             gpu_info = instance_type_info.get("GpuInfo", {})
             gpu, vram = gpu_info.get("Gpus", [{}])[0], gpu_info.get(
-                "TotalGpuMemoryInMiB"
+                "TotalGpuMemoryInMiB", 0
             )
+            architectures = instance_type_info.get("ProcessorInfo", {}).get(
+                "SupportedArchitectures", []
+            )
+            arch = architectures[0] if architectures else None
             return {
                 "cpu": instance_type_info.get("VCpuInfo", {}).get("DefaultVCpus"),
                 "memory": instance_type_info.get("MemoryInfo", {}).get("SizeInMiB"),
-                "gpu_count": gpu.get("Count"),
+                "gpu_count": gpu.get("Count", 0),
                 "vram": vram,
                 "gpu_manufacturer": gpu.get("Manufacturer"),
                 "gpu_name": gpu.get("Name"),
+                "arch": arch,
             }
     else:
         raise Exception(f"Unsupported provider: {provider}")
     raise Exception(f"Unsupported provider: {provider}")
+
+
+def camel_to_snake(camel_str: str) -> str:
+    kebab_case = camel_to_kebab(camel_str)
+    return kebab_case.replace("-", "_")
```

### Comparing `paka-0.1.8/pyproject.toml` & `paka-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "paka"
-version = "0.1.8"
+version = "0.1.9"
 description = "LLMOps tool designed to simplify the deployment and management of large language model (LLM) applications"
 homepage = "https://github.com/jjleng/paka"
 keywords = ["LLMOps", "RAG", "production", "Cloud"]
 authors = ["Jijun Leng"]
 readme = "README.md"
 
 [tool.codespell]
```

### Comparing `paka-0.1.8/PKG-INFO` & `paka-0.1.9/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paka
-Version: 0.1.8
+Version: 0.1.9
 Summary: LLMOps tool designed to simplify the deployment and management of large language model (LLM) applications
 Home-page: https://github.com/jjleng/paka
 Keywords: LLMOps,RAG,production,Cloud
 Author: Jijun Leng
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -30,118 +30,146 @@
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Requires-Dist: typer (>=0.12.3,<0.13.0)
 Requires-Dist: typing-extensions (>=4.11.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Welcome to Paka
 
-<img src="https://raw.githubusercontent.com/jjleng/paka/main/docs/img/paka.svg" alt="paka.svg" width="200" height="200">
+<img src="https://raw.githubusercontent.com/jjleng/paka/main/docs/img/paka.svg" alt="paka.png" width="100" height="100">
 
-**paka** is a versatile LLMOps tool that simplifies the deployment and management of large language model (LLM) apps with a single command.
 
-## Paka Highlights
+Get your LLM applications to the cloud with ease. Paka handles failure recovery, autoscaling, and monitoring, freeing you to concentrate on crafting your applications.
 
-- **Cloud-Agnostic Resource Provisioning**: paka starts by breaking down the barriers of cloud vendor lock-in, currently supporting EKS with plans to expand to more cloud services.
-- **Optimized Model Execution**: Designed for efficiency, paka runs LLM models on CPUs and Nvidia GPUs, ensuring optimal performance. Auto-scaling of model replicas based on CPU usage, request rate, and latency.
-- **Scalable Batch Job Management**: paka excels in managing batch jobs that dynamically scale out and in, catering to varying workload demands without manual intervention.
-- **Seamless Application Deployment**: With support for running Langchain and LlamaIndex applications as functions, paka offers scalability to zero and back up, along with rolling updates to ensure no downtime.
-- **Comprehensive Monitoring and Tracing**: Embedded with built-in support for metrics collection via Prometheus and Grafana, along with tracing through Zipkin.
+## 🚀 Bring LLM models to the cloud in minutes
+💰 Cut 50% cost with spot instances, backed by on-demand instances for reliable service quality.
 
+| Model      | Parameters | Quantization | GPU          | On-Demand | Spot    | AWS Node (us-west-2) |
+| ---------- | ---------- | ------------ | ------------ | --------- | ------- | ---------------------|
+| Llama 3    | 70B        | BF16         | A10G x 8     | $16.2880  | $4.8169 | g5.48xlarge          |
+| Llama 3    | 70B        | GPTQ 4bit    | T4 x 4       | $3.9120   | $1.6790 | g4dn.12xlarge        |
+| Llama 3    | 8B         | BF16         | L4 x 1       | $0.8048   | $0.1100 | g6.xlarge            |
+| Llama 2    | 7B         | GPTQ 4bit    | T4 x 1       | $0.526    | $0.2584 | g4dn.xlarge          |
+| Mistral    | 7B         | BF16         | T4 x 1       | $0.526    | $0.2584 | g4dn.xlarge          |
+| Phi3 Mini  | 3.8B       | BF16         | T4 x 1       | $0.526    | $0.2584 | g4dn.xlarge          |
 
+> Note: Prices are based on us-west-2 region and are in USD per hour. Spot prices change frequently.
+> See [Launch Templates](https://github.com/jjleng/paka/tree/main/examples/templates) for more details.
 
 
-### Runtime Inference
-Current runtime inference is done through the awesome [llama.cpp](https://github.com/ggerganov/llama.cpp) and [llama-cpp-python](https://github.com/abetlen/llama-cpp-python) projects.
+## 🏃 Effortlessly Launch RAG Applications
+You only need to take care of the application code. Build the RAG application with your favorite languages (python, TS) and frameworks (Langchain, LlamaIndex) and let Paka handles the rest.
 
-vLLM support is coming soon.
+### Support for Vector Store
+- A fast vector store (qdrant) for storing embeddings.
+- Tunable for performance and cost.
 
-Each model is ran in a separate model group. Each model group can have its own node type, replicas and autoscaling policies.
+### Serverless Deployment
+- Deploy your application as a serverless container.
+- Autoscaling and monitoring built-in.
 
-### Serverless Containers
-Applications are deployed as serverless containers using [knative](https://knative.dev). However, users can deploy their applications to the native cloud offerings as well, such as Lambda, Cloud Run, etc.
 
-### Batch Jobs
-Optional redis broker can be provisioned for celery jobs. Job workers are automatically scaled based on the queue length.
+## 📈 Monitoring
+Paka comes with built-in support for monitoring and tracing. Metrics are collected via Prometheus. Users can also enable Prometheus Alertmanager for alerting.
 
-### Vector Store
-Vector store is a key-value store for storing embeddings. Paka supports provisioning [qdrant](https://github.com/qdrant/qdrant).
+<div align="center" style="margin-top:20px;margin-bottom:20px;">
+<img src="https://raw.githubusercontent.com/jjleng/paka/main/docs/img/tokens_per_sec.png" max-width="1000"/>
+</div>
 
-### Monitoring
-Paka comes with built-in support for monitoring and tracing. Metrics are collected via Prometheus and Grafana, and tracing is done through Zipkin. Users can also enable Prometheus Alertmanager for alerting.
+## ⚙️ Architecture
 
-### Continuous Deployment
-Paka supports continuous deployment with rolling updates to ensure no downtime. Application can be built, pushed to container registry and deployed with a single command.
+<div align="center" style="margin-top:20px;margin-bottom:20px;">
+<img src="https://raw.githubusercontent.com/jjleng/paka/main/docs/img/architecture.png" max-width="1000"/>
+</div>
 
-### Building
-Application, job code is built using [buildpacks](https://buildpacks.io/). No need to write Dockerfile. However, user still needs to have docker runtime installed.
+## 📜 Roadmap
+- [x] (Multi-cloud) AWS support
+- [x] (Backend) vLLM
+- [x] (Backend) llama.cpp
+- [x] (Platform) Windows support
+- [x] (Accelerator) Nvidia GPU support
+- [ ] (Multi-cloud) GCP support
+- [ ] (Backend) TGI
+- [ ] (Accelerator) AMD GPU support
+- [ ] (Accelerator) Inferentia support
 
+## 🎬 Getting Started
+### Dependencies
+- docker daemon and CLI
+- AWS CLI
+```bash
+# Ensure your AWS credentials are correctly configured.
+aws configure
+```
 
-## Paka CLI Reference
-
-Install the paka CLI
+### Install Paka
 ```bash
 pip install paka
 ```
 
-### Provision a cluster
+### Provisioning the cluster
+
+Create a `cluster.yaml` file with the following content:
 
-Create a cluster.yaml
 ```yaml
+version: "1.2"
 aws:
   cluster:
-    name: example
+    name: my-awesome-cluster
     region: us-west-2
-    nodeType: t2.medium
+    namespace: default
+    nodeType: t3a.medium
     minNodes: 2
     maxNodes: 4
+  prometheus:
+    enabled: true
   modelGroups:
-    - nodeType: c7a.xlarge
+    - name: llama2-7b-chat
+      nodeType: g4dn.xlarge
+      isPublic: true
       minInstances: 1
-      maxInstances: 3
-      name: llama2-7b
-      resourceRequest:
-        cpu: 3600m
-        memory: 6Gi
-      autoScaleTriggers:
-        - type: cpu
-          metadata:
-            type: Utilization
-            value: "50"
+      maxInstances: 1
+      name: llama3-70b-instruct
+      runtime:
+        image: vllm/vllm-openai:v0.4.2
+      model:
+        hfRepoId: TheBloke/Llama-2-7B-Chat-GPTQ
+        useModelStore: false
+      gpu:
+        enabled: true
+        diskSize: 50
 ```
 
-Provision the cluster
+Bring up the cluster with the following command:
+
 ```bash
 paka cluster up -f cluster.yaml
 ```
 
-### Deploy an application
-Change to the application directory and add a `Procfile` and a .cnignore file.
-In `Procfile`, add the command to start the application. For example, for a flask app, it would be `web: gunicorn app:app`. In `.cnignore`, add the files to ignore during build.
+### Code up the application
+Use your favorite language and framework to build the application. Here is an example of a Python application using Langchain:
 
-To pin the version of the language runtime, add a `runtime.txt` file with the version number. For example, for python, it could be `python-3.11.*`.
+[invoice_extraction](https://github.com/jjleng/paka/tree/main/examples/invoice_extraction)
 
-For a python application, a requirements.txt file is required.
+With Paka, you can effortlessly build your source code and deploy it as a serverless function, no Dockerfile needed. Just ensure the following:
 
-To deploy the application, run `paka function deploy --name <function_name> --source <source_path> --entrypoint <Procfile_command>. For example:
+- **Procfile**: Defines the entrypoint for your application. See [Procfile](https://github.com/jjleng/paka/blob/main/examples/invoice_extraction/Procfile).
+- **.cnignore file**: Excludes any files that shouldn't be included in the build. See [.cnignore](https://github.com/jjleng/paka/blob/main/examples/invoice_extraction/.cnignore).
+- **runtime.txt**: Pins the version of the runtime your application uses. See [runtime.txt](https://github.com/jjleng/paka/blob/main/examples/invoice_extraction/runtime.txt).
+- **requirements.txt or package.json**: Lists all necessary packages for your application.
 
-```bash
-paka function deploy --name langchain-server --source . --entrypoint serve
-```
 
-### Destroy a cluster
+### Deploy the App
 ```bash
-paka cluster down -f cluster.yaml
+paka function deploy --name invoice-extraction --source . --entrypoint serve
 ```
 
+## 📖 Documentation
+
+- [Quick Start](./docs/quick_start.md)
+- [FAQ](./docs/faq.md)
+- [cluster_config.yaml](./docs/cluster_config.md)
+
 ## Contributing
 - code changes
 - `make check-all`
 - Open a PR
 
-## Dependencies
-- docker daemon and CLI
-- AWS CLI
-```bash
-# Ensure your AWS credentials are correctly configured.
-aws configure
-```
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

