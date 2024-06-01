# Comparing `tmp/neural_insights-2.4.tar.gz` & `tmp/neural_insights-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neural_insights-2.4.tar", last modified: Fri Dec 15 08:53:20 2023, max compression
+gzip compressed data, was "neural_insights-2.5.1.tar", last modified: Sat Jun  1 08:23:11 2024, max compression
```

## Comparing `neural_insights-2.4.tar` & `neural_insights-2.5.1.tar`

### file list

```diff
@@ -1,162 +1,162 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 08:53:20.209215 neural_insights-2.4/
--rw-r--r--   0 root         (0) root         (0)    11360 2023-12-15 08:47:06.000000 neural_insights-2.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)    12687 2023-12-15 08:53:20.209215 neural_insights-2.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11644 2023-12-15 08:47:06.000000 neural_insights-2.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 08:53:20.185213 neural_insights-2.4/neural_insights/
--rw-r--r--   0 root         (0) root         (0)      835 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 08:53:20.185213 neural_insights-2.4/neural_insights/bin/
--rw-r--r--   0 root         (0) root         (0)      688 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/bin/__init__.py
--rw-r--r--   0 root         (0) root         (0)      815 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/bin/neural_insights.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 08:53:20.185213 neural_insights-2.4/neural_insights/components/
--rw-r--r--   0 root         (0) root         (0)      707 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 08:53:20.185213 neural_insights-2.4/neural_insights/components/diagnosis/
--rw-r--r--   0 root         (0) root         (0)      711 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/diagnosis/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12439 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/diagnosis/diagnosis.py
--rw-r--r--   0 root         (0) root         (0)     2008 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/diagnosis/factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 08:53:20.185213 neural_insights-2.4/neural_insights/components/diagnosis/onnx_diagnosis/
--rw-r--r--   0 root         (0) root         (0)      718 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/diagnosis/onnx_diagnosis/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1703 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/diagnosis/onnx_diagnosis/onnxrt_diagnosis.py
--rw-r--r--   0 root         (0) root         (0)     2482 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/diagnosis/op_details.py
--rw-r--r--   0 root         (0) root         (0)     1490 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/diagnosis/op_entry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 08:53:20.185213 neural_insights-2.4/neural_insights/components/diagnosis/pytorch_diagnosis/
--rw-r--r--   0 root         (0) root         (0)      720 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/diagnosis/pytorch_diagnosis/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1706 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/diagnosis/pytorch_diagnosis/pytorch_diagnosis.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 08:53:20.185213 neural_insights-2.4/neural_insights/components/diagnosis/tensorflow_diagnosis/
--rw-r--r--   0 root         (0) root         (0)      722 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/diagnosis/tensorflow_diagnosis/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1731 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/diagnosis/tensorflow_diagnosis/tensorflow_diagnosis.py
--rw-r--r--   0 root         (0) root         (0)     2691 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/diagnosis/weights_details.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 08:53:20.185213 neural_insights-2.4/neural_insights/components/graph/
--rw-r--r--   0 root         (0) root         (0)      682 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/graph/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1021 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/graph/attribute.py
--rw-r--r--   0 root         (0) root         (0)     5012 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/graph/collapser.py
--rw-r--r--   0 root         (0) root         (0)     1205 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/graph/edge.py
--rw-r--r--   0 root         (0) root         (0)     3073 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/graph/graph.py
--rw-r--r--   0 root         (0) root         (0)     2301 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/graph/graph_reader.py
--rw-r--r--   0 root         (0) root         (0)     1840 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/graph/node.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 08:53:20.189213 neural_insights-2.4/neural_insights/components/graph/reader/
--rw-r--r--   0 root         (0) root         (0)      645 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/graph/reader/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8862 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/graph/reader/onnxrt_reader.py
--rw-r--r--   0 root         (0) root         (0)     1103 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/graph/reader/pytorch_reader.py
--rw-r--r--   0 root         (0) root         (0)     5117 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/graph/reader/tensorflow_reader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 08:53:20.189213 neural_insights-2.4/neural_insights/components/model/
--rw-r--r--   0 root         (0) root         (0)      695 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1092 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/model/domain.py
--rw-r--r--   0 root         (0) root         (0)     4954 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/model/model.py
--rw-r--r--   0 root         (0) root         (0)     1187 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/model/model_type_getter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 08:53:20.189213 neural_insights-2.4/neural_insights/components/model/onnxrt/
--rw-r--r--   0 root         (0) root         (0)      636 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/model/onnxrt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8692 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/model/onnxrt/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 08:53:20.189213 neural_insights-2.4/neural_insights/components/model/pytorch/
--rw-r--r--   0 root         (0) root         (0)      637 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/model/pytorch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1715 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/model/pytorch/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 08:53:20.189213 neural_insights-2.4/neural_insights/components/model/pytorch/pytorch_script/
--rw-r--r--   0 root         (0) root         (0)      637 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/model/pytorch/pytorch_script/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1887 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/model/pytorch/pytorch_script/model.py
--rw-r--r--   0 root         (0) root         (0)     3253 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/model/repository.py
--rw-r--r--   0 root         (0) root         (0)     1385 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/model/shape.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 08:53:20.189213 neural_insights-2.4/neural_insights/components/model/tensorflow/
--rw-r--r--   0 root         (0) root         (0)      640 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/model/tensorflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1175 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/model/tensorflow/frozen_pb.py
--rw-r--r--   0 root         (0) root         (0)     1288 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/model/tensorflow/keras.py
--rw-r--r--   0 root         (0) root         (0)     1513 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/model/tensorflow/meta_graph.py
--rw-r--r--   0 root         (0) root         (0)     4610 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/model/tensorflow/model.py
--rw-r--r--   0 root         (0) root         (0)     1045 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/model/tensorflow/saved_model.py
--rw-r--r--   0 root         (0) root         (0)     2386 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/model/tensorflow/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 08:53:20.189213 neural_insights-2.4/neural_insights/components/workload_manager/
--rw-r--r--   0 root         (0) root         (0)      718 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/workload_manager/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3123 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/workload_manager/quantization_workload.py
--rw-r--r--   0 root         (0) root         (0)     3529 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/workload_manager/workload.py
--rw-r--r--   0 root         (0) root         (0)     6971 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/components/workload_manager/workload_manager.py
--rw-r--r--   0 root         (0) root         (0)     1808 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/main.py
--rw-r--r--   0 root         (0) root         (0)     2789 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/ni.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 08:53:20.189213 neural_insights-2.4/neural_insights/test/
--rw-r--r--   0 root         (0) root         (0)      669 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 08:53:20.189213 neural_insights-2.4/neural_insights/test/components/
--rw-r--r--   0 root         (0) root         (0)      686 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/test/components/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 08:53:20.189213 neural_insights-2.4/neural_insights/test/components/graph/
--rw-r--r--   0 root         (0) root         (0)      682 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/test/components/graph/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2071 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/test/components/graph/test_attribute.py
--rw-r--r--   0 root         (0) root         (0)     5366 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/test/components/graph/test_collapser.py
--rw-r--r--   0 root         (0) root         (0)     2209 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/test/components/graph/test_edge.py
--rw-r--r--   0 root         (0) root         (0)     6066 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/test/components/graph/test_graph.py
--rw-r--r--   0 root         (0) root         (0)     2196 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/test/components/graph/test_graph_reader.py
--rw-r--r--   0 root         (0) root         (0)     1223 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/test/components/graph/test_node.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 08:53:20.189213 neural_insights-2.4/neural_insights/test/components/model/
--rw-r--r--   0 root         (0) root         (0)      686 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/test/components/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 08:53:20.189213 neural_insights-2.4/neural_insights/test/components/model/onnx/
--rw-r--r--   0 root         (0) root         (0)      690 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/test/components/model/onnx/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4620 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/test/components/model/onnx/test_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 08:53:20.193214 neural_insights-2.4/neural_insights/test/components/model/tensorflow/
--rw-r--r--   0 root         (0) root         (0)      702 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/test/components/model/tensorflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8318 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/test/components/model/tensorflow/test_frozen_pb.py
--rw-r--r--   0 root         (0) root         (0)     3840 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/test/components/model/tensorflow/test_keras.py
--rw-r--r--   0 root         (0) root         (0)     4259 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/test/components/model/tensorflow/test_meta_graph.py
--rw-r--r--   0 root         (0) root         (0)     4196 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/test/components/model/tensorflow/test_saved_model.py
--rw-r--r--   0 root         (0) root         (0)     1971 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/test/components/model/test_domain.py
--rw-r--r--   0 root         (0) root         (0)     2231 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/test/components/model/test_repository.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 08:53:20.193214 neural_insights-2.4/neural_insights/test/utils/
--rw-r--r--   0 root         (0) root         (0)      676 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/test/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2672 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/test/utils/test_expiring_dict.py
--rw-r--r--   0 root         (0) root         (0)     3344 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/test/utils/test_json_serializer.py
--rw-r--r--   0 root         (0) root         (0)     1006 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/test/utils/test_logger.py
--rw-r--r--   0 root         (0) root         (0)     3292 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/test/utils/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 08:53:20.193214 neural_insights-2.4/neural_insights/utils/
--rw-r--r--   0 root         (0) root         (0)      698 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1540 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/utils/consts.py
--rw-r--r--   0 root         (0) root         (0)     1551 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/utils/environment.py
--rw-r--r--   0 root         (0) root         (0)      959 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/utils/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2045 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/utils/expiring_dict.py
--rw-r--r--   0 root         (0) root         (0)     4838 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/utils/json_serializer.py
--rw-r--r--   0 root         (0) root         (0)     1024 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/utils/logger.py
--rw-r--r--   0 root         (0) root         (0)     1029 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/utils/singleton.py
--rw-r--r--   0 root         (0) root         (0)     2970 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/utils/utils.py
--rw-r--r--   0 root         (0) root         (0)      740 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 08:53:20.193214 neural_insights-2.4/neural_insights/web/
--rw-r--r--   0 root         (0) root         (0)      709 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/web/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 08:53:20.193214 neural_insights-2.4/neural_insights/web/app/
--rw-r--r--   0 root         (0) root         (0)     1271 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/web/app/asset-manifest.json
--rw-r--r--   0 root         (0) root         (0)    24484 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/web/app/favicon.ico
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 08:53:20.193214 neural_insights-2.4/neural_insights/web/app/icons/
--rw-r--r--   0 root         (0) root         (0)     1118 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/web/app/icons/057a-trash-solid-red.svg
--rw-r--r--   0 root         (0) root         (0)     1118 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/web/app/icons/057a-trash-solid.svg
--rw-r--r--   0 root         (0) root         (0)      776 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/web/app/icons/146b-copy-outlined-gray.svg
--rw-r--r--   0 root         (0) root         (0)      776 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/web/app/icons/146b-copy-outlined.svg
--rw-r--r--   0 root         (0) root         (0)      556 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/web/app/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 08:53:20.185213 neural_insights-2.4/neural_insights/web/app/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 08:53:20.193214 neural_insights-2.4/neural_insights/web/app/static/css/
--rw-r--r--   0 root         (0) root         (0)   246328 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/web/app/static/css/main.bb4c518c.css
--rw-r--r--   0 root         (0) root         (0)   560831 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/web/app/static/css/main.bb4c518c.css.map
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 08:53:20.201214 neural_insights-2.4/neural_insights/web/app/static/js/
--rw-r--r--   0 root         (0) root         (0)     4587 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/web/app/static/js/787.c1112931.chunk.js
--rw-r--r--   0 root         (0) root         (0)    10592 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/web/app/static/js/787.c1112931.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)  5737548 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/web/app/static/js/main.b053b871.js
--rw-r--r--   0 root         (0) root         (0)     3682 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/web/app/static/js/main.b053b871.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)  7112830 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/web/app/static/js/main.b053b871.js.map
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 08:53:20.205215 neural_insights-2.4/neural_insights/web/app/static/media/
--rw-r--r--   0 root         (0) root         (0)   312920 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/web/app/static/media/IntelClear_Bd.060888be7dccf869db54.ttf
--rw-r--r--   0 root         (0) root         (0)   314244 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/web/app/static/media/IntelClear_Lt.c5e18e9d5505364da760.ttf
--rw-r--r--   0 root         (0) root         (0)   316572 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/web/app/static/media/IntelClear_Rg.33af11200cffaf9540ff.ttf
--rw-r--r--   0 root         (0) root         (0)    96764 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/web/app/static/media/intelone-display-bold.64a6eab04dcda9c570c8.ttf
--rw-r--r--   0 root         (0) root         (0)   100524 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/web/app/static/media/intelone-display-light.68a9d0311f7374acb0cf.ttf
--rw-r--r--   0 root         (0) root         (0)    95288 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/web/app/static/media/intelone-display-regular.0f8c3ef25c545acb6b7c.ttf
--rw-r--r--   0 root         (0) root         (0)    64104 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/web/app/static/media/intelone-mono-font-family-regular.de914c9a804c00b4f3e5.ttf
--rw-r--r--   0 root         (0) root         (0)     2858 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/web/communication.py
--rw-r--r--   0 root         (0) root         (0)     9133 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/web/configuration.py
--rw-r--r--   0 root         (0) root         (0)      793 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/web/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     9504 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/web/router.py
--rw-r--r--   0 root         (0) root         (0)     8003 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/web/server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 08:53:20.205215 neural_insights-2.4/neural_insights/web/service/
--rw-r--r--   0 root         (0) root         (0)      627 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/web/service/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1067 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/web/service/request_data_processor.py
--rw-r--r--   0 root         (0) root         (0)     1838 2023-12-15 08:47:06.000000 neural_insights-2.4/neural_insights/web/service/response_generator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 08:53:20.185213 neural_insights-2.4/neural_insights.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12687 2023-12-15 08:53:20.000000 neural_insights-2.4/neural_insights.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6281 2023-12-15 08:53:20.000000 neural_insights-2.4/neural_insights.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-15 08:53:20.000000 neural_insights-2.4/neural_insights.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       80 2023-12-15 08:53:20.000000 neural_insights-2.4/neural_insights.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      138 2023-12-15 08:53:20.000000 neural_insights-2.4/neural_insights.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-12-15 08:53:20.000000 neural_insights-2.4/neural_insights.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2418 2023-12-15 08:47:06.000000 neural_insights-2.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      102 2023-12-15 08:53:20.209215 neural_insights-2.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     7117 2023-12-15 08:47:06.000000 neural_insights-2.4/setup.py
--rw-r--r--   0 root         (0) root         (0)    95719 2023-12-15 08:47:06.000000 neural_insights-2.4/third-party-programs.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:23:11.315732 neural_insights-2.5.1/
+-rw-r--r--   0 root         (0) root         (0)    11360 2024-06-01 08:22:37.000000 neural_insights-2.5.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    15142 2024-06-01 08:23:11.315732 neural_insights-2.5.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14096 2024-06-01 08:22:37.000000 neural_insights-2.5.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:23:11.285731 neural_insights-2.5.1/neural_insights/
+-rw-r--r--   0 root         (0) root         (0)      835 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:23:11.286731 neural_insights-2.5.1/neural_insights/bin/
+-rw-r--r--   0 root         (0) root         (0)      688 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/bin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      815 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/bin/neural_insights.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:23:11.286731 neural_insights-2.5.1/neural_insights/components/
+-rw-r--r--   0 root         (0) root         (0)      707 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:23:11.287731 neural_insights-2.5.1/neural_insights/components/diagnosis/
+-rw-r--r--   0 root         (0) root         (0)      711 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/diagnosis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12439 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/diagnosis/diagnosis.py
+-rw-r--r--   0 root         (0) root         (0)     2008 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/diagnosis/factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:23:11.287731 neural_insights-2.5.1/neural_insights/components/diagnosis/onnx_diagnosis/
+-rw-r--r--   0 root         (0) root         (0)      718 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/diagnosis/onnx_diagnosis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1703 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/diagnosis/onnx_diagnosis/onnxrt_diagnosis.py
+-rw-r--r--   0 root         (0) root         (0)     2482 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/diagnosis/op_details.py
+-rw-r--r--   0 root         (0) root         (0)     1490 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/diagnosis/op_entry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:23:11.287731 neural_insights-2.5.1/neural_insights/components/diagnosis/pytorch_diagnosis/
+-rw-r--r--   0 root         (0) root         (0)      720 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/diagnosis/pytorch_diagnosis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1706 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/diagnosis/pytorch_diagnosis/pytorch_diagnosis.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:23:11.288731 neural_insights-2.5.1/neural_insights/components/diagnosis/tensorflow_diagnosis/
+-rw-r--r--   0 root         (0) root         (0)      722 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/diagnosis/tensorflow_diagnosis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1731 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/diagnosis/tensorflow_diagnosis/tensorflow_diagnosis.py
+-rw-r--r--   0 root         (0) root         (0)     2691 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/diagnosis/weights_details.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:23:11.289731 neural_insights-2.5.1/neural_insights/components/graph/
+-rw-r--r--   0 root         (0) root         (0)      682 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/graph/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1021 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/graph/attribute.py
+-rw-r--r--   0 root         (0) root         (0)     5012 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/graph/collapser.py
+-rw-r--r--   0 root         (0) root         (0)     1205 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/graph/edge.py
+-rw-r--r--   0 root         (0) root         (0)     3073 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/graph/graph.py
+-rw-r--r--   0 root         (0) root         (0)     2301 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/graph/graph_reader.py
+-rw-r--r--   0 root         (0) root         (0)     1840 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/graph/node.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:23:11.289731 neural_insights-2.5.1/neural_insights/components/graph/reader/
+-rw-r--r--   0 root         (0) root         (0)      645 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/graph/reader/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8862 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/graph/reader/onnxrt_reader.py
+-rw-r--r--   0 root         (0) root         (0)     1103 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/graph/reader/pytorch_reader.py
+-rw-r--r--   0 root         (0) root         (0)     5117 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/graph/reader/tensorflow_reader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:23:11.290731 neural_insights-2.5.1/neural_insights/components/model/
+-rw-r--r--   0 root         (0) root         (0)      695 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1092 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/model/domain.py
+-rw-r--r--   0 root         (0) root         (0)     4954 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/model/model.py
+-rw-r--r--   0 root         (0) root         (0)     1187 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/model/model_type_getter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:23:11.290731 neural_insights-2.5.1/neural_insights/components/model/onnxrt/
+-rw-r--r--   0 root         (0) root         (0)      636 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/model/onnxrt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8692 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/model/onnxrt/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:23:11.291731 neural_insights-2.5.1/neural_insights/components/model/pytorch/
+-rw-r--r--   0 root         (0) root         (0)      637 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/model/pytorch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1715 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/model/pytorch/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:23:11.291731 neural_insights-2.5.1/neural_insights/components/model/pytorch/pytorch_script/
+-rw-r--r--   0 root         (0) root         (0)      637 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/model/pytorch/pytorch_script/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1887 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/model/pytorch/pytorch_script/model.py
+-rw-r--r--   0 root         (0) root         (0)     3253 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/model/repository.py
+-rw-r--r--   0 root         (0) root         (0)     1385 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/model/shape.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:23:11.292731 neural_insights-2.5.1/neural_insights/components/model/tensorflow/
+-rw-r--r--   0 root         (0) root         (0)      640 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/model/tensorflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1175 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/model/tensorflow/frozen_pb.py
+-rw-r--r--   0 root         (0) root         (0)     1288 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/model/tensorflow/keras.py
+-rw-r--r--   0 root         (0) root         (0)     1513 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/model/tensorflow/meta_graph.py
+-rw-r--r--   0 root         (0) root         (0)     4610 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/model/tensorflow/model.py
+-rw-r--r--   0 root         (0) root         (0)     1045 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/model/tensorflow/saved_model.py
+-rw-r--r--   0 root         (0) root         (0)     2386 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/model/tensorflow/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:23:11.292731 neural_insights-2.5.1/neural_insights/components/workload_manager/
+-rw-r--r--   0 root         (0) root         (0)      718 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/workload_manager/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3123 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/workload_manager/quantization_workload.py
+-rw-r--r--   0 root         (0) root         (0)     3529 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/workload_manager/workload.py
+-rw-r--r--   0 root         (0) root         (0)     6971 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/components/workload_manager/workload_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1808 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/main.py
+-rw-r--r--   0 root         (0) root         (0)     2789 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/ni.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:23:11.292731 neural_insights-2.5.1/neural_insights/test/
+-rw-r--r--   0 root         (0) root         (0)      669 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:23:11.293731 neural_insights-2.5.1/neural_insights/test/components/
+-rw-r--r--   0 root         (0) root         (0)      686 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/test/components/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:23:11.293731 neural_insights-2.5.1/neural_insights/test/components/graph/
+-rw-r--r--   0 root         (0) root         (0)      682 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/test/components/graph/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2071 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/test/components/graph/test_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     5366 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/test/components/graph/test_collapser.py
+-rw-r--r--   0 root         (0) root         (0)     2209 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/test/components/graph/test_edge.py
+-rw-r--r--   0 root         (0) root         (0)     6066 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/test/components/graph/test_graph.py
+-rw-r--r--   0 root         (0) root         (0)     2196 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/test/components/graph/test_graph_reader.py
+-rw-r--r--   0 root         (0) root         (0)     1223 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/test/components/graph/test_node.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:23:11.294731 neural_insights-2.5.1/neural_insights/test/components/model/
+-rw-r--r--   0 root         (0) root         (0)      686 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/test/components/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:23:11.294731 neural_insights-2.5.1/neural_insights/test/components/model/onnx/
+-rw-r--r--   0 root         (0) root         (0)      690 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/test/components/model/onnx/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4620 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/test/components/model/onnx/test_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:23:11.295731 neural_insights-2.5.1/neural_insights/test/components/model/tensorflow/
+-rw-r--r--   0 root         (0) root         (0)      702 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/test/components/model/tensorflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8318 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/test/components/model/tensorflow/test_frozen_pb.py
+-rw-r--r--   0 root         (0) root         (0)     3840 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/test/components/model/tensorflow/test_keras.py
+-rw-r--r--   0 root         (0) root         (0)     4259 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/test/components/model/tensorflow/test_meta_graph.py
+-rw-r--r--   0 root         (0) root         (0)     4196 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/test/components/model/tensorflow/test_saved_model.py
+-rw-r--r--   0 root         (0) root         (0)     1971 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/test/components/model/test_domain.py
+-rw-r--r--   0 root         (0) root         (0)     2231 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/test/components/model/test_repository.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:23:11.295731 neural_insights-2.5.1/neural_insights/test/utils/
+-rw-r--r--   0 root         (0) root         (0)      676 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/test/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2672 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/test/utils/test_expiring_dict.py
+-rw-r--r--   0 root         (0) root         (0)     3344 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/test/utils/test_json_serializer.py
+-rw-r--r--   0 root         (0) root         (0)     1006 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/test/utils/test_logger.py
+-rw-r--r--   0 root         (0) root         (0)     3292 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/test/utils/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:23:11.297731 neural_insights-2.5.1/neural_insights/utils/
+-rw-r--r--   0 root         (0) root         (0)      698 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1540 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/utils/consts.py
+-rw-r--r--   0 root         (0) root         (0)     1551 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/utils/environment.py
+-rw-r--r--   0 root         (0) root         (0)      959 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/utils/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2045 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/utils/expiring_dict.py
+-rw-r--r--   0 root         (0) root         (0)     4838 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/utils/json_serializer.py
+-rw-r--r--   0 root         (0) root         (0)     1024 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/utils/logger.py
+-rw-r--r--   0 root         (0) root         (0)     1029 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/utils/singleton.py
+-rw-r--r--   0 root         (0) root         (0)     2970 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/utils/utils.py
+-rw-r--r--   0 root         (0) root         (0)      740 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:23:11.297731 neural_insights-2.5.1/neural_insights/web/
+-rw-r--r--   0 root         (0) root         (0)      709 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/web/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:23:11.298731 neural_insights-2.5.1/neural_insights/web/app/
+-rw-r--r--   0 root         (0) root         (0)     1271 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/web/app/asset-manifest.json
+-rw-r--r--   0 root         (0) root         (0)    24484 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/web/app/favicon.ico
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:23:11.298731 neural_insights-2.5.1/neural_insights/web/app/icons/
+-rw-r--r--   0 root         (0) root         (0)     1118 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/web/app/icons/057a-trash-solid-red.svg
+-rw-r--r--   0 root         (0) root         (0)     1118 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/web/app/icons/057a-trash-solid.svg
+-rw-r--r--   0 root         (0) root         (0)      776 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/web/app/icons/146b-copy-outlined-gray.svg
+-rw-r--r--   0 root         (0) root         (0)      776 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/web/app/icons/146b-copy-outlined.svg
+-rw-r--r--   0 root         (0) root         (0)      556 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/web/app/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:23:11.283731 neural_insights-2.5.1/neural_insights/web/app/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:23:11.299731 neural_insights-2.5.1/neural_insights/web/app/static/css/
+-rw-r--r--   0 root         (0) root         (0)   246328 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/web/app/static/css/main.bb4c518c.css
+-rw-r--r--   0 root         (0) root         (0)   560831 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/web/app/static/css/main.bb4c518c.css.map
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:23:11.305732 neural_insights-2.5.1/neural_insights/web/app/static/js/
+-rw-r--r--   0 root         (0) root         (0)     4587 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/web/app/static/js/787.c1112931.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    10592 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/web/app/static/js/787.c1112931.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)  5737548 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/web/app/static/js/main.b053b871.js
+-rw-r--r--   0 root         (0) root         (0)     3682 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/web/app/static/js/main.b053b871.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)  7112830 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/web/app/static/js/main.b053b871.js.map
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:23:11.314732 neural_insights-2.5.1/neural_insights/web/app/static/media/
+-rw-r--r--   0 root         (0) root         (0)   312920 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/web/app/static/media/IntelClear_Bd.060888be7dccf869db54.ttf
+-rw-r--r--   0 root         (0) root         (0)   314244 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/web/app/static/media/IntelClear_Lt.c5e18e9d5505364da760.ttf
+-rw-r--r--   0 root         (0) root         (0)   316572 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/web/app/static/media/IntelClear_Rg.33af11200cffaf9540ff.ttf
+-rw-r--r--   0 root         (0) root         (0)    96764 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/web/app/static/media/intelone-display-bold.64a6eab04dcda9c570c8.ttf
+-rw-r--r--   0 root         (0) root         (0)   100524 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/web/app/static/media/intelone-display-light.68a9d0311f7374acb0cf.ttf
+-rw-r--r--   0 root         (0) root         (0)    95288 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/web/app/static/media/intelone-display-regular.0f8c3ef25c545acb6b7c.ttf
+-rw-r--r--   0 root         (0) root         (0)    64104 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/web/app/static/media/intelone-mono-font-family-regular.de914c9a804c00b4f3e5.ttf
+-rw-r--r--   0 root         (0) root         (0)     2858 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/web/communication.py
+-rw-r--r--   0 root         (0) root         (0)     9708 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/web/configuration.py
+-rw-r--r--   0 root         (0) root         (0)      793 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/web/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     9504 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/web/router.py
+-rw-r--r--   0 root         (0) root         (0)     8005 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/web/server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:23:11.315732 neural_insights-2.5.1/neural_insights/web/service/
+-rw-r--r--   0 root         (0) root         (0)      627 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/web/service/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1067 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/web/service/request_data_processor.py
+-rw-r--r--   0 root         (0) root         (0)     1838 2024-06-01 08:22:38.000000 neural_insights-2.5.1/neural_insights/web/service/response_generator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:23:11.315732 neural_insights-2.5.1/neural_insights.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15142 2024-06-01 08:23:11.000000 neural_insights-2.5.1/neural_insights.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6281 2024-06-01 08:23:11.000000 neural_insights-2.5.1/neural_insights.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-01 08:23:11.000000 neural_insights-2.5.1/neural_insights.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2024-06-01 08:23:11.000000 neural_insights-2.5.1/neural_insights.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      138 2024-06-01 08:23:11.000000 neural_insights-2.5.1/neural_insights.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-06-01 08:23:11.000000 neural_insights-2.5.1/neural_insights.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2418 2024-06-01 08:22:38.000000 neural_insights-2.5.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      102 2024-06-01 08:23:11.315732 neural_insights-2.5.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8675 2024-06-01 08:22:38.000000 neural_insights-2.5.1/setup.py
+-rw-r--r--   0 root         (0) root         (0)    95740 2024-06-01 08:22:38.000000 neural_insights-2.5.1/third-party-programs.txt
```

### Comparing `neural_insights-2.4/LICENSE` & `neural_insights-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/PKG-INFO` & `neural_insights-2.5.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,110 +1,135 @@
-Metadata-Version: 2.1
-Name: neural_insights
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
-Requires-Dist: cryptography
-Requires-Dist: Flask
-Requires-Dist: Flask-Cors
-Requires-Dist: Flask-SocketIO
-Requires-Dist: gevent
-Requires-Dist: gevent-websocket
-Requires-Dist: neural_compressor>=2.2
-Requires-Dist: pywin32; sys_platform != "linux"
-Requires-Dist: torchinfo
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

### Comparing `neural_insights-2.4/README.md` & `neural_insights-2.5.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,83 +1,162 @@
+Metadata-Version: 2.1
+Name: neural_insights
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
+Requires-Dist: cryptography
+Requires-Dist: Flask
+Requires-Dist: Flask-Cors
+Requires-Dist: Flask-SocketIO
+Requires-Dist: gevent
+Requires-Dist: gevent-websocket
+Requires-Dist: neural_compressor>=2.2
+Requires-Dist: pywin32; sys_platform != "linux"
+Requires-Dist: torchinfo
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

### Comparing `neural_insights-2.4/neural_insights/__init__.py` & `neural_insights-2.5.1/neural_insights/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/bin/__init__.py` & `neural_insights-2.5.1/neural_insights/bin/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/bin/neural_insights.py` & `neural_insights-2.5.1/neural_insights/bin/neural_insights.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/__init__.py` & `neural_insights-2.5.1/neural_insights/components/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/diagnosis/__init__.py` & `neural_insights-2.5.1/neural_insights/components/diagnosis/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/diagnosis/diagnosis.py` & `neural_insights-2.5.1/neural_insights/components/diagnosis/diagnosis.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/diagnosis/factory.py` & `neural_insights-2.5.1/neural_insights/components/diagnosis/factory.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/diagnosis/onnx_diagnosis/__init__.py` & `neural_insights-2.5.1/neural_insights/components/diagnosis/onnx_diagnosis/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/diagnosis/onnx_diagnosis/onnxrt_diagnosis.py` & `neural_insights-2.5.1/neural_insights/components/diagnosis/onnx_diagnosis/onnxrt_diagnosis.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/diagnosis/op_details.py` & `neural_insights-2.5.1/neural_insights/components/diagnosis/op_details.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/diagnosis/op_entry.py` & `neural_insights-2.5.1/neural_insights/components/diagnosis/op_entry.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/diagnosis/pytorch_diagnosis/__init__.py` & `neural_insights-2.5.1/neural_insights/components/diagnosis/pytorch_diagnosis/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/diagnosis/pytorch_diagnosis/pytorch_diagnosis.py` & `neural_insights-2.5.1/neural_insights/components/diagnosis/pytorch_diagnosis/pytorch_diagnosis.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/diagnosis/tensorflow_diagnosis/__init__.py` & `neural_insights-2.5.1/neural_insights/components/diagnosis/tensorflow_diagnosis/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/diagnosis/tensorflow_diagnosis/tensorflow_diagnosis.py` & `neural_insights-2.5.1/neural_insights/components/diagnosis/tensorflow_diagnosis/tensorflow_diagnosis.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/diagnosis/weights_details.py` & `neural_insights-2.5.1/neural_insights/components/diagnosis/weights_details.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/graph/__init__.py` & `neural_insights-2.5.1/neural_insights/components/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/graph/attribute.py` & `neural_insights-2.5.1/neural_insights/components/graph/attribute.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/graph/collapser.py` & `neural_insights-2.5.1/neural_insights/components/graph/collapser.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/graph/edge.py` & `neural_insights-2.5.1/neural_insights/components/graph/edge.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/graph/graph.py` & `neural_insights-2.5.1/neural_insights/components/graph/graph.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/graph/graph_reader.py` & `neural_insights-2.5.1/neural_insights/components/graph/graph_reader.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/graph/node.py` & `neural_insights-2.5.1/neural_insights/components/graph/node.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/graph/reader/__init__.py` & `neural_insights-2.5.1/neural_insights/components/graph/reader/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/graph/reader/onnxrt_reader.py` & `neural_insights-2.5.1/neural_insights/components/graph/reader/onnxrt_reader.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/graph/reader/pytorch_reader.py` & `neural_insights-2.5.1/neural_insights/components/graph/reader/pytorch_reader.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/graph/reader/tensorflow_reader.py` & `neural_insights-2.5.1/neural_insights/components/graph/reader/tensorflow_reader.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/model/__init__.py` & `neural_insights-2.5.1/neural_insights/components/model/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/model/domain.py` & `neural_insights-2.5.1/neural_insights/components/model/domain.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/model/model.py` & `neural_insights-2.5.1/neural_insights/components/model/model.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/model/model_type_getter.py` & `neural_insights-2.5.1/neural_insights/components/model/model_type_getter.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/model/onnxrt/__init__.py` & `neural_insights-2.5.1/neural_insights/components/model/onnxrt/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/model/onnxrt/model.py` & `neural_insights-2.5.1/neural_insights/components/model/onnxrt/model.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/model/pytorch/__init__.py` & `neural_insights-2.5.1/neural_insights/components/model/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/model/pytorch/model.py` & `neural_insights-2.5.1/neural_insights/components/model/pytorch/model.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/model/pytorch/pytorch_script/__init__.py` & `neural_insights-2.5.1/neural_insights/components/model/pytorch/pytorch_script/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/model/pytorch/pytorch_script/model.py` & `neural_insights-2.5.1/neural_insights/components/model/pytorch/pytorch_script/model.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/model/repository.py` & `neural_insights-2.5.1/neural_insights/components/model/repository.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/model/shape.py` & `neural_insights-2.5.1/neural_insights/components/model/shape.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/model/tensorflow/__init__.py` & `neural_insights-2.5.1/neural_insights/components/model/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/model/tensorflow/frozen_pb.py` & `neural_insights-2.5.1/neural_insights/components/model/tensorflow/frozen_pb.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/model/tensorflow/keras.py` & `neural_insights-2.5.1/neural_insights/components/model/tensorflow/keras.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/model/tensorflow/meta_graph.py` & `neural_insights-2.5.1/neural_insights/components/model/tensorflow/meta_graph.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/model/tensorflow/model.py` & `neural_insights-2.5.1/neural_insights/components/model/tensorflow/model.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/model/tensorflow/saved_model.py` & `neural_insights-2.5.1/neural_insights/components/model/tensorflow/saved_model.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/model/tensorflow/utils.py` & `neural_insights-2.5.1/neural_insights/components/model/tensorflow/utils.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/workload_manager/__init__.py` & `neural_insights-2.5.1/neural_insights/components/workload_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/workload_manager/quantization_workload.py` & `neural_insights-2.5.1/neural_insights/components/workload_manager/quantization_workload.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/workload_manager/workload.py` & `neural_insights-2.5.1/neural_insights/components/workload_manager/workload.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/components/workload_manager/workload_manager.py` & `neural_insights-2.5.1/neural_insights/components/workload_manager/workload_manager.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/main.py` & `neural_insights-2.5.1/neural_insights/main.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/ni.py` & `neural_insights-2.5.1/neural_insights/ni.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/test/__init__.py` & `neural_insights-2.5.1/neural_insights/test/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/test/components/__init__.py` & `neural_insights-2.5.1/neural_insights/test/components/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/test/components/graph/__init__.py` & `neural_insights-2.5.1/neural_insights/test/components/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/test/components/graph/test_attribute.py` & `neural_insights-2.5.1/neural_insights/test/components/graph/test_attribute.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/test/components/graph/test_collapser.py` & `neural_insights-2.5.1/neural_insights/test/components/graph/test_collapser.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/test/components/graph/test_edge.py` & `neural_insights-2.5.1/neural_insights/test/components/graph/test_edge.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/test/components/graph/test_graph.py` & `neural_insights-2.5.1/neural_insights/test/components/graph/test_graph.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/test/components/graph/test_graph_reader.py` & `neural_insights-2.5.1/neural_insights/test/components/graph/test_graph_reader.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/test/components/graph/test_node.py` & `neural_insights-2.5.1/neural_insights/test/components/graph/test_node.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/test/components/model/__init__.py` & `neural_insights-2.5.1/neural_insights/test/components/model/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/test/components/model/onnx/__init__.py` & `neural_insights-2.5.1/neural_insights/test/components/model/onnx/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/test/components/model/onnx/test_model.py` & `neural_insights-2.5.1/neural_insights/test/components/model/onnx/test_model.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/test/components/model/tensorflow/__init__.py` & `neural_insights-2.5.1/neural_insights/test/components/model/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/test/components/model/tensorflow/test_frozen_pb.py` & `neural_insights-2.5.1/neural_insights/test/components/model/tensorflow/test_frozen_pb.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/test/components/model/tensorflow/test_keras.py` & `neural_insights-2.5.1/neural_insights/test/components/model/tensorflow/test_keras.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/test/components/model/tensorflow/test_meta_graph.py` & `neural_insights-2.5.1/neural_insights/test/components/model/tensorflow/test_meta_graph.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/test/components/model/tensorflow/test_saved_model.py` & `neural_insights-2.5.1/neural_insights/test/components/model/tensorflow/test_saved_model.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/test/components/model/test_domain.py` & `neural_insights-2.5.1/neural_insights/test/components/model/test_domain.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/test/components/model/test_repository.py` & `neural_insights-2.5.1/neural_insights/test/components/model/test_repository.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/test/utils/__init__.py` & `neural_insights-2.5.1/neural_insights/test/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/test/utils/test_expiring_dict.py` & `neural_insights-2.5.1/neural_insights/test/utils/test_expiring_dict.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/test/utils/test_json_serializer.py` & `neural_insights-2.5.1/neural_insights/test/utils/test_json_serializer.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/test/utils/test_logger.py` & `neural_insights-2.5.1/neural_insights/test/utils/test_logger.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/test/utils/test_utils.py` & `neural_insights-2.5.1/neural_insights/test/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/utils/__init__.py` & `neural_insights-2.5.1/neural_insights/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/utils/consts.py` & `neural_insights-2.5.1/neural_insights/utils/consts.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/utils/environment.py` & `neural_insights-2.5.1/neural_insights/utils/environment.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/utils/exceptions.py` & `neural_insights-2.5.1/neural_insights/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/utils/expiring_dict.py` & `neural_insights-2.5.1/neural_insights/utils/expiring_dict.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/utils/json_serializer.py` & `neural_insights-2.5.1/neural_insights/utils/json_serializer.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/utils/logger.py` & `neural_insights-2.5.1/neural_insights/utils/logger.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/utils/singleton.py` & `neural_insights-2.5.1/neural_insights/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/utils/utils.py` & `neural_insights-2.5.1/neural_insights/utils/utils.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/version.py` & `neural_insights-2.5.1/neural_insights/version.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/web/__init__.py` & `neural_insights-2.5.1/neural_insights/web/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/web/app/asset-manifest.json` & `neural_insights-2.5.1/neural_insights/web/app/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/web/app/favicon.ico` & `neural_insights-2.5.1/neural_insights/web/app/favicon.ico`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/web/app/icons/057a-trash-solid-red.svg` & `neural_insights-2.5.1/neural_insights/web/app/icons/057a-trash-solid-red.svg`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/web/app/icons/057a-trash-solid.svg` & `neural_insights-2.5.1/neural_insights/web/app/icons/057a-trash-solid.svg`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/web/app/icons/146b-copy-outlined-gray.svg` & `neural_insights-2.5.1/neural_insights/web/app/icons/146b-copy-outlined-gray.svg`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/web/app/icons/146b-copy-outlined.svg` & `neural_insights-2.5.1/neural_insights/web/app/icons/146b-copy-outlined.svg`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/web/app/index.html` & `neural_insights-2.5.1/neural_insights/web/app/index.html`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/web/app/static/css/main.bb4c518c.css` & `neural_insights-2.5.1/neural_insights/web/app/static/css/main.bb4c518c.css`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/web/app/static/css/main.bb4c518c.css.map` & `neural_insights-2.5.1/neural_insights/web/app/static/css/main.bb4c518c.css.map`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/web/app/static/js/787.c1112931.chunk.js` & `neural_insights-2.5.1/neural_insights/web/app/static/js/787.c1112931.chunk.js`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/web/app/static/js/787.c1112931.chunk.js.map` & `neural_insights-2.5.1/neural_insights/web/app/static/js/787.c1112931.chunk.js.map`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/web/app/static/js/main.b053b871.js` & `neural_insights-2.5.1/neural_insights/web/app/static/js/main.b053b871.js`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/web/app/static/js/main.b053b871.js.LICENSE.txt` & `neural_insights-2.5.1/neural_insights/web/app/static/js/main.b053b871.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/web/app/static/js/main.b053b871.js.map` & `neural_insights-2.5.1/neural_insights/web/app/static/js/main.b053b871.js.map`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/web/app/static/media/IntelClear_Bd.060888be7dccf869db54.ttf` & `neural_insights-2.5.1/neural_insights/web/app/static/media/IntelClear_Bd.060888be7dccf869db54.ttf`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/web/app/static/media/IntelClear_Lt.c5e18e9d5505364da760.ttf` & `neural_insights-2.5.1/neural_insights/web/app/static/media/IntelClear_Lt.c5e18e9d5505364da760.ttf`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/web/app/static/media/IntelClear_Rg.33af11200cffaf9540ff.ttf` & `neural_insights-2.5.1/neural_insights/web/app/static/media/IntelClear_Rg.33af11200cffaf9540ff.ttf`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/web/app/static/media/intelone-display-bold.64a6eab04dcda9c570c8.ttf` & `neural_insights-2.5.1/neural_insights/web/app/static/media/intelone-display-bold.64a6eab04dcda9c570c8.ttf`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/web/app/static/media/intelone-display-light.68a9d0311f7374acb0cf.ttf` & `neural_insights-2.5.1/neural_insights/web/app/static/media/intelone-display-light.68a9d0311f7374acb0cf.ttf`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/web/app/static/media/intelone-display-regular.0f8c3ef25c545acb6b7c.ttf` & `neural_insights-2.5.1/neural_insights/web/app/static/media/intelone-display-regular.0f8c3ef25c545acb6b7c.ttf`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/web/app/static/media/intelone-mono-font-family-regular.de914c9a804c00b4f3e5.ttf` & `neural_insights-2.5.1/neural_insights/web/app/static/media/intelone-mono-font-family-regular.de914c9a804c00b4f3e5.ttf`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/web/communication.py` & `neural_insights-2.5.1/neural_insights/web/communication.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/web/configuration.py` & `neural_insights-2.5.1/neural_insights/web/configuration.py`

 * *Files 7% similar despite different names*

```diff
@@ -222,43 +222,66 @@
             base_url = f"{base_url}{self.url_prefix}"
         return f"{base_url}/?token={self.token}"
 
     def dump_token_to_file(self) -> None:
         """Dump token to file."""
         token_filepath = os.path.join(WORKDIR_LOCATION, "token")
         os.makedirs(os.path.dirname(token_filepath), exist_ok=True)
-        with open(token_filepath, "w") as token_file:
-            token_file.write(self.token)
 
         if sys.platform == "win32":
-            import ntsecuritycon as con  # pylint: disable=import-error
-            import win32api  # pylint: disable=import-error
-            import win32security  # pylint: disable=import-error
-
-            user, _, _ = win32security.LookupAccountName("", win32api.GetUserName())
-            security_descriptor = win32security.GetFileSecurity(
-                token_filepath,
-                win32security.DACL_SECURITY_INFORMATION,
-            )
-            dacl = win32security.ACL()
-            dacl.AddAccessAllowedAce(
-                win32security.ACL_REVISION,
-                con.FILE_GENERIC_READ | con.FILE_GENERIC_WRITE,
-                user,
-            )
-            security_descriptor.SetSecurityDescriptorDacl(1, dacl, 0)
-            win32security.SetFileSecurity(
-                token_filepath,
-                win32security.DACL_SECURITY_INFORMATION,
-                security_descriptor,
-            )
-        else:
-            os.chown(token_filepath, uid=os.geteuid(), gid=os.getgid())
-            os.chmod(token_filepath, 0o600)
+            self.create_secured_token_file_win(token_filepath)
+
+        try:
+            token_file = os.open(token_filepath, flags=os.O_WRONLY | os.O_CREAT, mode=0o600)
+            os.write(token_file, self.token.encode())
+        except Exception as err:
+            raise err
+        finally:
+            os.close(token_file)
+
         log.debug(f"Token has been dumped to {token_filepath}.")
 
+    @staticmethod
+    def create_secured_token_file_win(token_filepath: str):
+        """Create secured file on Windows OS."""
+        import ntsecuritycon as con  # pylint: disable=import-error
+        import win32api  # pylint: disable=import-error
+        import win32file  # pylint: disable=import-error
+        import win32security  # pylint: disable=import-error
+
+        username = win32api.GetUserName()
+        os.makedirs(os.path.dirname(token_filepath), exist_ok=True)
+
+        if os.path.exists(token_filepath):
+            os.remove(token_filepath)
+
+        security_descriptor = win32security.SECURITY_DESCRIPTOR()
+        user_sid, _, _ = win32security.LookupAccountName("", username)
+
+        access_rights = con.FILE_ALL_ACCESS
+
+        dacl = win32security.ACL()
+        dacl.AddAccessAllowedAce(win32security.ACL_REVISION, access_rights, user_sid)
+
+        security_descriptor.SetSecurityDescriptorDacl(1, dacl, 0)
+
+        security_attributes = win32security.SECURITY_ATTRIBUTES()
+        security_attributes.SECURITY_DESCRIPTOR = security_descriptor
+
+        handle = win32file.CreateFile(
+            token_filepath,
+            win32file.GENERIC_WRITE,
+            win32file.FILE_SHARE_READ,
+            security_attributes,
+            win32file.CREATE_NEW,
+            win32file.FILE_ATTRIBUTE_NORMAL,
+            None,
+        )
+
+        win32file.CloseHandle(handle)
+
     def _ensure_valid_port(self, port: int) -> None:
         """Validate if proposed port number is allowed by TCP/IP."""
         if port < 1:
             raise ValueError(f"Lowest allowed port number is 1, attempted to use: {port}")
         if port > 65535:
             raise ValueError(f"Highest allowed port number is 65535, attempted to use: {port}")
```

### Comparing `neural_insights-2.4/neural_insights/web/exceptions.py` & `neural_insights-2.5.1/neural_insights/web/exceptions.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/web/router.py` & `neural_insights-2.5.1/neural_insights/web/router.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/web/server.py` & `neural_insights-2.5.1/neural_insights/web/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,17 +115,17 @@
     }
 
 
 @app_blueprint.after_request
 def block_iframe(response: WebResponse) -> WebResponse:
     """Block iframe and set others CSP."""
     response.headers["X-Frame-Options"] = "DENY"
-    response.headers[
-        "Content-Security-Policy"
-    ] = "frame-ancestors 'none'; font-src 'self'; img-src 'self'; script-src 'self'"
+    response.headers["Content-Security-Policy"] = (
+        "frame-ancestors 'none'; font-src 'self'; img-src 'self'; script-src 'self'"
+    )
     response.headers["Access-Control-Max-Age"] = "-1"
     return response
 
 
 @app_blueprint.after_request
 def block_sniffing(response: WebResponse) -> WebResponse:
     """Block MIME sniffing."""
```

### Comparing `neural_insights-2.4/neural_insights/web/service/__init__.py` & `neural_insights-2.5.1/neural_insights/web/service/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/web/service/request_data_processor.py` & `neural_insights-2.5.1/neural_insights/web/service/request_data_processor.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights/web/service/response_generator.py` & `neural_insights-2.5.1/neural_insights/web/service/response_generator.py`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/neural_insights.egg-info/PKG-INFO` & `neural_insights-2.5.1/neural_insights.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: neural-insights
-Version: 2.4
+Name: neural_insights
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
@@ -28,83 +28,135 @@
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

### Comparing `neural_insights-2.4/neural_insights.egg-info/SOURCES.txt` & `neural_insights-2.5.1/neural_insights.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/pyproject.toml` & `neural_insights-2.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `neural_insights-2.4/third-party-programs.txt` & `neural_insights-2.5.1/third-party-programs.txt`

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

