# Comparing `tmp/onediff-1.1.0.dev202405300128.tar.gz` & `tmp/onediff-1.1.0.dev202405310129.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onediff-1.1.0.dev202405300128.tar", last modified: Thu May 30 01:28:43 2024, max compression
+gzip compressed data, was "onediff-1.1.0.dev202405310129.tar", last modified: Fri May 31 01:29:11 2024, max compression
```

## Comparing `onediff-1.1.0.dev202405300128.tar` & `onediff-1.1.0.dev202405310129.tar`

### file list

```diff
@@ -1,97 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:28:43.519402 onediff-1.1.0.dev202405300128/
--rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-05-30 01:28:43.519402 onediff-1.1.0.dev202405300128/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13557 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 01:28:43.519402 onediff-1.1.0.dev202405300128/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:28:43.503402 onediff-1.1.0.dev202405300128/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:28:43.507402 onediff-1.1.0.dev202405300128/src/infer_compiler_registry/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/infer_compiler_registry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:28:43.507402 onediff-1.1.0.dev202405300128/src/infer_compiler_registry/register_diffusers/
--rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/infer_compiler_registry/register_diffusers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    77125 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/infer_compiler_registry/register_diffusers/attention_processor_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/infer_compiler_registry/register_diffusers/resnet_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    24024 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/infer_compiler_registry/register_diffusers/spatio_temporal_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    61005 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/infer_compiler_registry/register_diffusers/transformer_2d_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    14699 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/infer_compiler_registry/register_diffusers/unet_2d_blocks_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    24118 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/infer_compiler_registry/register_diffusers/unet_2d_condition_oflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:28:43.507402 onediff-1.1.0.dev202405300128/src/infer_compiler_registry/register_diffusers_enterprise_lite/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/infer_compiler_registry/register_diffusers_enterprise_lite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:28:43.507402 onediff-1.1.0.dev202405300128/src/infer_compiler_registry/register_onediff_quant/
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/infer_compiler_registry/register_onediff_quant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:28:43.507402 onediff-1.1.0.dev202405300128/src/onediff/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:28:43.511402 onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:28:43.511402 onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/deployable_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:28:43.511402 onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/nexfort/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/nexfort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/nexfort/deployable_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/nexfort/nexfort.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:28:43.511402 onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/args_tree_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    10228 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/deployable_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     7017 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/dual_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/env_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/graph_management_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:28:43.515402 onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/import_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/import_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6835 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/import_tools/dyn_mock_mod.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/import_tools/format_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/import_tools/import_module_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/import_tools/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/import_tools/patch_for_compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/oneflow.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/oneflow_exec_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/online_quantization_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/param_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:28:43.515402 onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/transform/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15062 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/transform/builtin_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/transform/custom_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/transform/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/transform/patch_for_comfy.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/transform/patch_for_diffusers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:28:43.515402 onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/utils/cost_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/utils/version_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:28:43.515402 onediff-1.1.0.dev202405300128/src/onediff/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/optimization/attention_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/optimization/quant_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/optimization/rewrite_self_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:28:43.515402 onediff-1.1.0.dev202405300128/src/onediff/quantization/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/quantization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/quantization/load_quantized_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/quantization/quant_pipeline_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/quantization/quantize_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/quantization/quantize_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:28:43.515402 onediff-1.1.0.dev202405300128/src/onediff/schedulers/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/schedulers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:28:43.515402 onediff-1.1.0.dev202405300128/src/onediff/torch_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/torch_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6862 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/torch_utils/model_inplace_assign.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/torch_utils/module_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:28:43.519402 onediff-1.1.0.dev202405300128/src/onediff/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/utils/env_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/src/onediff/utils/log_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:28:43.519402 onediff-1.1.0.dev202405300128/src/onediff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-05-30 01:28:43.000000 onediff-1.1.0.dev202405300128/src/onediff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-05-30 01:28:43.000000 onediff-1.1.0.dev202405300128/src/onediff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 01:28:43.000000 onediff-1.1.0.dev202405300128/src/onediff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-30 01:28:43.000000 onediff-1.1.0.dev202405300128/src/onediff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-30 01:28:43.000000 onediff-1.1.0.dev202405300128/src/onediff.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:28:43.519402 onediff-1.1.0.dev202405300128/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/tests/test_dual_module_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/tests/test_pipelines_oneflow_img2img.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/tests/test_quantitative_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-30 01:28:37.000000 onediff-1.1.0.dev202405300128/tests/test_quantize_custom_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:29:11.335000 onediff-1.1.0.dev202405310129/
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-05-31 01:29:11.335000 onediff-1.1.0.dev202405310129/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13557 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 01:29:11.335000 onediff-1.1.0.dev202405310129/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:29:11.319000 onediff-1.1.0.dev202405310129/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:29:11.323000 onediff-1.1.0.dev202405310129/src/infer_compiler_registry/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/infer_compiler_registry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:29:11.323000 onediff-1.1.0.dev202405310129/src/infer_compiler_registry/register_diffusers/
+-rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/infer_compiler_registry/register_diffusers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77125 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/infer_compiler_registry/register_diffusers/attention_processor_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/infer_compiler_registry/register_diffusers/resnet_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24024 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/infer_compiler_registry/register_diffusers/spatio_temporal_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61005 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/infer_compiler_registry/register_diffusers/transformer_2d_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14699 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/infer_compiler_registry/register_diffusers/unet_2d_blocks_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24118 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/infer_compiler_registry/register_diffusers/unet_2d_condition_oflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:29:11.323000 onediff-1.1.0.dev202405310129/src/infer_compiler_registry/register_diffusers_enterprise_lite/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/infer_compiler_registry/register_diffusers_enterprise_lite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:29:11.323000 onediff-1.1.0.dev202405310129/src/infer_compiler_registry/register_onediff_quant/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/infer_compiler_registry/register_onediff_quant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:29:11.323000 onediff-1.1.0.dev202405310129/src/onediff/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:29:11.323000 onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:29:11.323000 onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/deployable_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:29:11.327000 onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/nexfort/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/nexfort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/nexfort/deployable_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/nexfort/nexfort.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:29:11.327000 onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/args_tree_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10362 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/deployable_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7017 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/dual_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6884 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/env_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/graph_management_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:29:11.327000 onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/import_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/import_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6835 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/import_tools/dyn_mock_mod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/import_tools/format_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/import_tools/import_module_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/import_tools/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/import_tools/patch_for_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/oneflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/oneflow_exec_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/online_quantization_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/param_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:29:11.331000 onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/transform/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15062 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/transform/builtin_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/transform/custom_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/transform/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/transform/patch_for_comfy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/transform/patch_for_diffusers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:29:11.331000 onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/utils/cost_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/utils/hash_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/utils/version_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:29:11.331000 onediff-1.1.0.dev202405310129/src/onediff/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/optimization/attention_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/optimization/quant_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/optimization/rewrite_self_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:29:11.331000 onediff-1.1.0.dev202405310129/src/onediff/quantization/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/quantization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/quantization/load_quantized_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/quantization/quant_pipeline_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/quantization/quantize_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/quantization/quantize_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:29:11.331000 onediff-1.1.0.dev202405310129/src/onediff/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/schedulers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:29:11.331000 onediff-1.1.0.dev202405310129/src/onediff/torch_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/torch_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6862 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/torch_utils/model_inplace_assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/torch_utils/module_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:29:11.335000 onediff-1.1.0.dev202405310129/src/onediff/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/utils/env_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/src/onediff/utils/log_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:29:11.335000 onediff-1.1.0.dev202405310129/src/onediff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-05-31 01:29:11.000000 onediff-1.1.0.dev202405310129/src/onediff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-05-31 01:29:11.000000 onediff-1.1.0.dev202405310129/src/onediff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 01:29:11.000000 onediff-1.1.0.dev202405310129/src/onediff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-31 01:29:11.000000 onediff-1.1.0.dev202405310129/src/onediff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-31 01:29:11.000000 onediff-1.1.0.dev202405310129/src/onediff.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:29:11.335000 onediff-1.1.0.dev202405310129/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/tests/test_dual_module_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/tests/test_pipelines_oneflow_img2img.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/tests/test_quantitative_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-31 01:29:01.000000 onediff-1.1.0.dev202405310129/tests/test_quantize_custom_model.py
```

### Comparing `onediff-1.1.0.dev202405300128/LICENSE` & `onediff-1.1.0.dev202405310129/LICENSE`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405300128/PKG-INFO` & `onediff-1.1.0.dev202405310129/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onediff
-Version: 1.1.0.dev202405300128
+Version: 1.1.0.dev202405310129
 Summary: an out-of-the-box acceleration library for diffusion models
 Home-page: https://github.com/siliconflow/onediff
 Author: OneDiff contributors
 Author-email: contact@siliconflow.com
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: onediff Version: 1.1.0.dev202405300128 Summary: an
+Metadata-Version: 2.1 Name: onediff Version: 1.1.0.dev202405310129 Summary: an
 out-of-the-box acceleration library for diffusion models Home-page: https://
 github.com/siliconflow/onediff Author: OneDiff contributors Author-email:
 contact@siliconflow.com License: Apache-2.0 Classifier: Development Status :: 5
 - Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Education Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
```

### Comparing `onediff-1.1.0.dev202405300128/README.md` & `onediff-1.1.0.dev202405310129/README.md`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405300128/setup.py` & `onediff-1.1.0.dev202405310129/setup.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405300128/src/infer_compiler_registry/register_diffusers/__init__.py` & `onediff-1.1.0.dev202405310129/src/infer_compiler_registry/register_diffusers/__init__.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405300128/src/infer_compiler_registry/register_diffusers/attention_processor_oflow.py` & `onediff-1.1.0.dev202405310129/src/infer_compiler_registry/register_diffusers/attention_processor_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405300128/src/infer_compiler_registry/register_diffusers/resnet_oflow.py` & `onediff-1.1.0.dev202405310129/src/infer_compiler_registry/register_diffusers/resnet_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405300128/src/infer_compiler_registry/register_diffusers/spatio_temporal_oflow.py` & `onediff-1.1.0.dev202405310129/src/infer_compiler_registry/register_diffusers/spatio_temporal_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405300128/src/infer_compiler_registry/register_diffusers/transformer_2d_oflow.py` & `onediff-1.1.0.dev202405310129/src/infer_compiler_registry/register_diffusers/transformer_2d_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405300128/src/infer_compiler_registry/register_diffusers/unet_2d_blocks_oflow.py` & `onediff-1.1.0.dev202405310129/src/infer_compiler_registry/register_diffusers/unet_2d_blocks_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405300128/src/infer_compiler_registry/register_diffusers/unet_2d_condition_oflow.py` & `onediff-1.1.0.dev202405310129/src/infer_compiler_registry/register_diffusers/unet_2d_condition_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405300128/src/infer_compiler_registry/register_diffusers_enterprise_lite/__init__.py` & `onediff-1.1.0.dev202405310129/src/infer_compiler_registry/register_diffusers_enterprise_lite/__init__.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405300128/src/infer_compiler_registry/register_onediff_quant/__init__.py` & `onediff-1.1.0.dev202405310129/src/infer_compiler_registry/register_onediff_quant/__init__.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/compiler.py` & `onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/compiler.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/nexfort/deployable_module.py` & `onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/nexfort/deployable_module.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/nexfort/nexfort.py` & `onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/nexfort/nexfort.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/args_tree_util.py` & `onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/args_tree_util.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,55 @@
 import torch
 import oneflow as flow
 from oneflow.framework.args_tree import ArgsTree
 from onediff.utils import logger
 
+from .utils.hash_utils import generate_input_structure_key
+
 
 def input_output_processor(func):
     def process_input(*args, **kwargs):
         def input_fn(value):
             if isinstance(value, torch.Tensor):
                 # TODO: https://github.com/siliconflow/sd-team/issues/109
                 return flow.utils.tensor.from_torch(value.contiguous())
             else:
                 return value
 
         args_tree = ArgsTree((args, kwargs), False, tensor_type=torch.Tensor)
-        input_count = len(
-            [v for v in args_tree.iter_nodes() if isinstance(v, torch.Tensor)]
-        )
+
+        input_structure_key = generate_input_structure_key(args_tree)
         out = args_tree.map_leaf(input_fn)
         mapped_args = out[0]
         mapped_kwargs = out[1]
-        return mapped_args, mapped_kwargs, input_count
+        return mapped_args, mapped_kwargs, input_structure_key
 
     def process_output(output):
         def output_fn(value):
             if isinstance(value, flow.Tensor):
                 return flow.utils.tensor.to_torch(value)
             else:
                 return value
 
         out_tree = ArgsTree((output, None), False)
         out = out_tree.map_leaf(output_fn)
         return out[0]
 
-    def wrapper(self: "DeployableModule", *args, **kwargs):
-        mapped_args, mapped_kwargs, input_count = process_input(*args, **kwargs)
+    def wrapper(self: "OneflowDeployableModule", *args, **kwargs):
+        mapped_args, mapped_kwargs, input_structure_key = process_input(*args, **kwargs)
         if (
             self._deployable_module_options.use_graph
+            and self._deployable_module_enable_dynamic
             and self._deployable_module_dpl_graph is not None
+            and self._deployable_module_input_structure_key != input_structure_key
         ):
-            count = len(self._deployable_module_dpl_graph._input_op_names)
-            if count != input_count:
-                logger.warning(
-                    f"Module {type(self._deployable_module_model.oneflow_module)} input tensor count changed from {count} to {input_count}, will compile again."
-                )
-                self._deployable_module_dpl_graph = None
-                self._load_graph_first_run = True
+            logger.warning(
+                "Input structure key has changed. Resetting the deployable module graph."
+            )
+            self._deployable_module_dpl_graph = None
+            self._load_graph_first_run = True
+            self._deployable_module_input_structure_key = None
 
         output = func(self, *mapped_args, **mapped_kwargs)
         return process_output(output)
 
     return wrapper
```

### Comparing `onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/deployable_module.py` & `onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/deployable_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,28 +68,29 @@
         self._deployable_module_quant_config = None
         self._deployable_module_options = (
             options if options is not None else OneflowCompileOptions()
         )
         self._deployable_module_dpl_graph = None
         self._is_raw_deployable_module = True
         self._load_graph_first_run = True
+        self._deployable_module_input_structure_key = None
 
     @classmethod
     def from_existing(cls, existing_module, dynamic=True, options=None):
         torch_module = existing_module._deployable_module_model._torch_module
         oneflow_module = existing_module._deployable_module_model._oneflow_module
         instance = cls(torch_module, oneflow_module, dynamic, options)
         instance._deployable_module_dpl_graph = None
         if hasattr(existing_module, "_deployable_module_dpl_graph"):
             instance._deployable_module_dpl_graph = (
                 existing_module._deployable_module_dpl_graph
             )
         instance._load_graph_first_run = existing_module._load_graph_first_run
-        instance._deployable_module_input_count = (
-            existing_module._deployable_module_input_count
+        instance._deployable_module_input_structure_key = (
+            existing_module._deployable_module_input_structure_key
         )
         instance._deployable_module_quant_config = (
             existing_module._deployable_module_quant_config
         )
 
         return instance
 
@@ -207,14 +208,15 @@
             return
         self._deployable_module_options.graph_file = file_path
         self._clear_old_graph()
 
     def _clear_old_graph(self):
         self._load_graph_first_run = True
         self._deployable_module_dpl_graph = None
+        self._deployable_module_input_structure_key = None
         del self._deployable_module_model.oneflow_module
 
     def get_graph_file(self):
         return self._deployable_module_options.graph_file
 
     def apply_online_quant(self, quant_config):
         """
```

### Comparing `onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/dual_module.py` & `onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/dual_module.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/env_var.py` & `onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/env_var.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 class OneflowCompileOptions:
     dynamic: bool = True
     use_graph: bool = True
     debug_level: int = -1
     max_cached_graph_size: int = 9
     graph_file: str = None
     graph_file_device: torch.device = None
-
     # Optimization related environment variables
     run_graph_by_vm: bool = None
     graph_delay_variable_op_execution: bool = None
 
     conv_allow_half_precision_accumulation: bool = None
     matmul_allow_half_precision_accumulation: bool = None
     attention_allow_half_precision_accumulation: bool = None
```

### Comparing `onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/graph.py` & `onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/graph.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/import_tools/dyn_mock_mod.py` & `onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/import_tools/dyn_mock_mod.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/import_tools/format_utils.py` & `onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/import_tools/format_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/import_tools/import_module_utils.py` & `onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/import_tools/import_module_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/import_tools/importer.py` & `onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/import_tools/importer.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/import_tools/patch_for_compiler.py` & `onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/import_tools/patch_for_compiler.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/oneflow.py` & `onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/oneflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/oneflow_exec_mode.py` & `onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/oneflow_exec_mode.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/online_quantization_utils.py` & `onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/online_quantization_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/param_utils.py` & `onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/param_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/transform/builtin_transform.py` & `onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/transform/builtin_transform.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/transform/custom_transform.py` & `onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/transform/custom_transform.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """A module for registering custom torch2oflow functions and classes."""
 import inspect
 import importlib.util
 from pathlib import Path
+import sys
 from typing import Callable, Dict, List, Optional, Union
 from ..import_tools import import_module_from_path
 from .manager import transform_mgr
 from .builtin_transform import torch2oflow
 from onediff.utils import logger
 
 __all__ = ["register"]
@@ -47,28 +48,31 @@
             import_module_from_path(module_path)
         except Exception as e:
             logger.warning(f"Failed to import {module_name} from {module_path}. {e=}")
 
     # compiler_registry_path
     registry_path = Path(__file__).parents[5] / "infer_compiler_registry"
 
-    if importlib.util.find_spec("diffusers") is not None:
-        import_module_safely(registry_path / "register_diffusers", "register_diffusers")
+    if sys.modules.get("diffusers") is not None:
+        if importlib.util.find_spec("diffusers") is not None:
+            import_module_safely(
+                registry_path / "register_diffusers", "register_diffusers"
+            )
+
+        if importlib.util.find_spec("diffusers_enterprise_lite"):
+            import_module_safely(
+                registry_path / "register_diffusers_enterprise_lite",
+                "register_diffusers_enterprise_lite",
+            )
 
     if importlib.util.find_spec("onediff_quant") is not None:
         import_module_safely(
             registry_path / "register_onediff_quant", "register_onediff_quant"
         )
 
-    if importlib.util.find_spec("diffusers_enterprise_lite") is not None:
-        import_module_safely(
-            registry_path / "register_diffusers_enterprise_lite",
-            "register_diffusers_enterprise_lite",
-        )
-
 
 def ensure_list(obj):
     if isinstance(obj, list):
         return obj
     return [obj]
```

### Comparing `onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/transform/manager.py` & `onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/transform/manager.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/transform/patch_for_comfy.py` & `onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/transform/patch_for_comfy.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/transform/patch_for_diffusers.py` & `onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/transform/patch_for_diffusers.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/utils/cost_util.py` & `onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/utils/cost_util.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/oneflow/utils/version_util.py` & `onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/oneflow/utils/version_util.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405300128/src/onediff/infer_compiler/backends/registry.py` & `onediff-1.1.0.dev202405310129/src/onediff/infer_compiler/backends/registry.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405300128/src/onediff/optimization/attention_processor.py` & `onediff-1.1.0.dev202405310129/src/onediff/optimization/attention_processor.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405300128/src/onediff/optimization/quant_optimizer.py` & `onediff-1.1.0.dev202405310129/src/onediff/optimization/quant_optimizer.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405300128/src/onediff/optimization/rewrite_self_attention.py` & `onediff-1.1.0.dev202405310129/src/onediff/optimization/rewrite_self_attention.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405300128/src/onediff/quantization/load_quantized_model.py` & `onediff-1.1.0.dev202405310129/src/onediff/quantization/load_quantized_model.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405300128/src/onediff/quantization/quant_pipeline_test.py` & `onediff-1.1.0.dev202405310129/src/onediff/quantization/quant_pipeline_test.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405300128/src/onediff/quantization/quantize_pipeline.py` & `onediff-1.1.0.dev202405310129/src/onediff/quantization/quantize_pipeline.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405300128/src/onediff/quantization/quantize_utils.py` & `onediff-1.1.0.dev202405310129/src/onediff/quantization/quantize_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405300128/src/onediff/torch_utils/model_inplace_assign.py` & `onediff-1.1.0.dev202405310129/src/onediff/torch_utils/model_inplace_assign.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405300128/src/onediff/torch_utils/module_operations.py` & `onediff-1.1.0.dev202405310129/src/onediff/torch_utils/module_operations.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405300128/src/onediff/utils/env_var.py` & `onediff-1.1.0.dev202405310129/src/onediff/utils/env_var.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405300128/src/onediff/utils/log_utils.py` & `onediff-1.1.0.dev202405310129/src/onediff/utils/log_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,19 +25,21 @@
 
     def __getattr__(self, name):
         return getattr(self.logger, name)
 
     def configure_logging(self, name, level, log_dir=None, file_name=None):
         logger = logging.getLogger(name)
 
-        if logger.hasHandlers():
+        if logger.hasHandlers() and len(logger.handlers) > 0:
             logger.warning("Logging handlers already exist for %s", name)
             return
 
         logger.setLevel(level)
+        # Prevent messages from being propagated to the root logger
+        logger.propagate = False
 
         # Create a console formatter and add it to a console handler
         console_formatter = ColorFormatter(
             fmt="%(levelname)s [%(asctime)s] %(pathname)s:%(lineno)d - %(message)s",
             datefmt="%Y-%m-%d %H:%M:%S",
         )
```

### Comparing `onediff-1.1.0.dev202405300128/src/onediff.egg-info/PKG-INFO` & `onediff-1.1.0.dev202405310129/src/onediff.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onediff
-Version: 1.1.0.dev202405300128
+Version: 1.1.0.dev202405310129
 Summary: an out-of-the-box acceleration library for diffusion models
 Home-page: https://github.com/siliconflow/onediff
 Author: OneDiff contributors
 Author-email: contact@siliconflow.com
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: onediff Version: 1.1.0.dev202405300128 Summary: an
+Metadata-Version: 2.1 Name: onediff Version: 1.1.0.dev202405310129 Summary: an
 out-of-the-box acceleration library for diffusion models Home-page: https://
 github.com/siliconflow/onediff Author: OneDiff contributors Author-email:
 contact@siliconflow.com License: Apache-2.0 Classifier: Development Status :: 5
 - Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Education Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
```

### Comparing `onediff-1.1.0.dev202405300128/src/onediff.egg-info/SOURCES.txt` & `onediff-1.1.0.dev202405310129/src/onediff.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 src/onediff/infer_compiler/backends/oneflow/transform/builtin_transform.py
 src/onediff/infer_compiler/backends/oneflow/transform/custom_transform.py
 src/onediff/infer_compiler/backends/oneflow/transform/manager.py
 src/onediff/infer_compiler/backends/oneflow/transform/patch_for_comfy.py
 src/onediff/infer_compiler/backends/oneflow/transform/patch_for_diffusers.py
 src/onediff/infer_compiler/backends/oneflow/utils/__init__.py
 src/onediff/infer_compiler/backends/oneflow/utils/cost_util.py
+src/onediff/infer_compiler/backends/oneflow/utils/hash_utils.py
 src/onediff/infer_compiler/backends/oneflow/utils/version_util.py
 src/onediff/optimization/__init__.py
 src/onediff/optimization/attention_processor.py
 src/onediff/optimization/quant_optimizer.py
 src/onediff/optimization/rewrite_self_attention.py
 src/onediff/quantization/__init__.py
 src/onediff/quantization/load_quantized_model.py
```

### Comparing `onediff-1.1.0.dev202405300128/tests/test_dual_module_list.py` & `onediff-1.1.0.dev202405310129/tests/test_dual_module_list.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405300128/tests/test_pipelines_oneflow_img2img.py` & `onediff-1.1.0.dev202405310129/tests/test_pipelines_oneflow_img2img.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405300128/tests/test_quantitative_quality.py` & `onediff-1.1.0.dev202405310129/tests/test_quantitative_quality.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405300128/tests/test_quantize_custom_model.py` & `onediff-1.1.0.dev202405310129/tests/test_quantize_custom_model.py`

 * *Files identical despite different names*

