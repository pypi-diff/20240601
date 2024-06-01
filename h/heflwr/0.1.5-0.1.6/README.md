# Comparing `tmp/heflwr-0.1.5.tar.gz` & `tmp/heflwr-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heflwr-0.1.5.tar", last modified: Sun May 26 10:41:08 2024, max compression
+gzip compressed data, was "heflwr-0.1.6.tar", last modified: Sat Jun  1 12:58:02 2024, max compression
```

## Comparing `heflwr-0.1.5.tar` & `heflwr-0.1.6.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 10:41:08.746721 heflwr-0.1.5/
--rw-rw-rw-   0        0        0     1088 2024-05-14 16:05:22.000000 heflwr-0.1.5/LICENSE
--rw-rw-rw-   0        0        0       15 2024-05-14 16:05:22.000000 heflwr-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0      495 2024-05-26 10:41:08.745725 heflwr-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      183 2024-05-26 10:34:11.000000 heflwr-0.1.5/README.rst
--rw-rw-rw-   0        0        0       42 2024-05-26 10:41:08.746721 heflwr-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      608 2024-05-26 10:40:41.000000 heflwr-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-26 10:41:08.720599 heflwr-0.1.5/src/
-drwxrwxrwx   0        0        0        0 2024-05-26 10:41:08.725069 heflwr-0.1.5/src/heflwr/
--rw-rw-rw-   0        0        0      104 2024-05-26 10:40:41.000000 heflwr-0.1.5/src/heflwr/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-26 10:41:08.729454 heflwr-0.1.5/src/heflwr/fed/
--rw-rw-rw-   0        0        0       86 2024-05-26 07:46:59.000000 heflwr-0.1.5/src/heflwr/fed/__init__.py
--rw-rw-rw-   0        0        0     6697 2024-05-26 08:10:01.000000 heflwr-0.1.5/src/heflwr/fed/aggregate.py
--rw-rw-rw-   0        0        0     4782 2024-05-25 12:38:47.000000 heflwr-0.1.5/src/heflwr/fed/heflwr_aggregate.py
--rw-rw-rw-   0        0        0        0 2024-05-14 16:05:22.000000 heflwr-0.1.5/src/heflwr/fed/heflwr_client_manager.py
-drwxrwxrwx   0        0        0        0 2024-05-26 10:41:08.733125 heflwr-0.1.5/src/heflwr/log/
--rw-rw-rw-   0        0        0      116 2024-05-23 14:23:17.000000 heflwr-0.1.5/src/heflwr/log/__init__.py
--rw-rw-rw-   0        0        0     1396 2024-05-23 14:19:38.000000 heflwr-0.1.5/src/heflwr/log/configurator.py
--rw-rw-rw-   0        0        0      984 2024-05-23 14:03:31.000000 heflwr-0.1.5/src/heflwr/log/handlers.py
--rw-rw-rw-   0        0        0      661 2024-05-23 14:19:38.000000 heflwr-0.1.5/src/heflwr/log/log_info.py
-drwxrwxrwx   0        0        0        0 2024-05-26 10:41:08.733125 heflwr-0.1.5/src/heflwr/monitor/
--rw-rw-rw-   0        0        0       61 2024-05-14 16:05:22.000000 heflwr-0.1.5/src/heflwr/monitor/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-26 10:41:08.735854 heflwr-0.1.5/src/heflwr/monitor/process_monitor/
--rw-rw-rw-   0        0        0      133 2024-05-25 11:52:25.000000 heflwr-0.1.5/src/heflwr/monitor/process_monitor/__init__.py
--rw-rw-rw-   0        0        0     5523 2024-05-25 13:52:47.000000 heflwr-0.1.5/src/heflwr/monitor/process_monitor/file_monitor.py
--rw-rw-rw-   0        0        0     5542 2024-05-25 13:52:47.000000 heflwr-0.1.5/src/heflwr/monitor/process_monitor/prometheus_monitor.py
--rw-rw-rw-   0        0        0     5350 2024-05-25 13:52:47.000000 heflwr-0.1.5/src/heflwr/monitor/process_monitor/remote_monitor.py
-drwxrwxrwx   0        0        0        0 2024-05-26 10:41:08.738844 heflwr-0.1.5/src/heflwr/monitor/thread_monitor/
--rw-rw-rw-   0        0        0      133 2024-05-25 11:52:25.000000 heflwr-0.1.5/src/heflwr/monitor/thread_monitor/__init__.py
--rw-rw-rw-   0        0        0     4939 2024-05-25 13:52:47.000000 heflwr-0.1.5/src/heflwr/monitor/thread_monitor/file_monitor.py
--rw-rw-rw-   0        0        0     5300 2024-05-25 13:52:47.000000 heflwr-0.1.5/src/heflwr/monitor/thread_monitor/prometheus_monitor.py
--rw-rw-rw-   0        0        0     5019 2024-05-25 13:52:47.000000 heflwr-0.1.5/src/heflwr/monitor/thread_monitor/remote_monitor.py
-drwxrwxrwx   0        0        0        0 2024-05-26 10:41:08.740693 heflwr-0.1.5/src/heflwr/monitor/utils/
--rw-rw-rw-   0        0        0        0 2024-05-14 16:05:22.000000 heflwr-0.1.5/src/heflwr/monitor/utils/__init__.py
--rw-rw-rw-   0        0        0     1028 2024-05-14 16:05:22.000000 heflwr-0.1.5/src/heflwr/monitor/utils/network.py
--rw-rw-rw-   0        0        0     4500 2024-05-14 16:05:22.000000 heflwr-0.1.5/src/heflwr/monitor/utils/power.py
-drwxrwxrwx   0        0        0        0 2024-05-26 10:41:08.743726 heflwr-0.1.5/src/heflwr/nn/
--rw-rw-rw-   0        0        0      153 2024-05-14 16:05:22.000000 heflwr-0.1.5/src/heflwr/nn/__init__.py
--rw-rw-rw-   0        0        0      359 2024-05-19 19:11:39.000000 heflwr-0.1.5/src/heflwr/nn/scaler.py
--rw-rw-rw-   0        0        0     4840 2024-05-26 09:58:40.000000 heflwr-0.1.5/src/heflwr/nn/ssbatchnorm2d.py
--rw-rw-rw-   0        0        0     9704 2024-05-19 19:11:39.000000 heflwr-0.1.5/src/heflwr/nn/ssconv2d.py
--rw-rw-rw-   0        0        0     9292 2024-05-19 19:11:39.000000 heflwr-0.1.5/src/heflwr/nn/sslinear.py
-drwxrwxrwx   0        0        0        0 2024-05-26 10:41:08.727427 heflwr-0.1.5/src/heflwr.egg-info/
--rw-rw-rw-   0        0        0      495 2024-05-26 10:41:08.000000 heflwr-0.1.5/src/heflwr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1137 2024-05-26 10:41:08.000000 heflwr-0.1.5/src/heflwr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 10:41:08.000000 heflwr-0.1.5/src/heflwr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-26 10:41:08.000000 heflwr-0.1.5/src/heflwr.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-26 10:41:08.744728 heflwr-0.1.5/tests/
--rw-rw-rw-   0        0        0        0 2024-05-14 16:05:22.000000 heflwr-0.1.5/tests/test.py
+drwxrwxrwx   0        0        0        0 2024-06-01 12:58:02.131906 heflwr-0.1.6/
+-rw-rw-rw-   0        0        0     1088 2024-05-14 16:05:22.000000 heflwr-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0       15 2024-05-14 16:05:22.000000 heflwr-0.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      495 2024-06-01 12:58:02.131906 heflwr-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      183 2024-05-26 10:34:11.000000 heflwr-0.1.6/README.rst
+-rw-rw-rw-   0        0        0       42 2024-06-01 12:58:02.131906 heflwr-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      608 2024-06-01 12:57:59.000000 heflwr-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 12:58:02.105619 heflwr-0.1.6/src/
+drwxrwxrwx   0        0        0        0 2024-06-01 12:58:02.109791 heflwr-0.1.6/src/heflwr/
+-rw-rw-rw-   0        0        0      104 2024-06-01 12:57:59.000000 heflwr-0.1.6/src/heflwr/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 12:58:02.114194 heflwr-0.1.6/src/heflwr/fed/
+-rw-rw-rw-   0        0        0       86 2024-05-26 07:46:59.000000 heflwr-0.1.6/src/heflwr/fed/__init__.py
+-rw-rw-rw-   0        0        0     6697 2024-05-26 08:10:01.000000 heflwr-0.1.6/src/heflwr/fed/aggregate.py
+-rw-rw-rw-   0        0        0     4782 2024-05-25 12:38:47.000000 heflwr-0.1.6/src/heflwr/fed/heflwr_aggregate.py
+-rw-rw-rw-   0        0        0        0 2024-05-14 16:05:22.000000 heflwr-0.1.6/src/heflwr/fed/heflwr_client_manager.py
+drwxrwxrwx   0        0        0        0 2024-06-01 12:58:02.115395 heflwr-0.1.6/src/heflwr/log/
+-rw-rw-rw-   0        0        0      116 2024-05-23 14:23:17.000000 heflwr-0.1.6/src/heflwr/log/__init__.py
+-rw-rw-rw-   0        0        0     1396 2024-05-23 14:19:38.000000 heflwr-0.1.6/src/heflwr/log/configurator.py
+-rw-rw-rw-   0        0        0      984 2024-05-23 14:03:31.000000 heflwr-0.1.6/src/heflwr/log/handlers.py
+-rw-rw-rw-   0        0        0      661 2024-05-23 14:19:38.000000 heflwr-0.1.6/src/heflwr/log/log_info.py
+drwxrwxrwx   0        0        0        0 2024-06-01 12:58:02.116881 heflwr-0.1.6/src/heflwr/monitor/
+-rw-rw-rw-   0        0        0       61 2024-05-14 16:05:22.000000 heflwr-0.1.6/src/heflwr/monitor/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 12:58:02.120932 heflwr-0.1.6/src/heflwr/monitor/process_monitor/
+-rw-rw-rw-   0        0        0      133 2024-05-25 11:52:25.000000 heflwr-0.1.6/src/heflwr/monitor/process_monitor/__init__.py
+-rw-rw-rw-   0        0        0     5523 2024-05-25 13:52:47.000000 heflwr-0.1.6/src/heflwr/monitor/process_monitor/file_monitor.py
+-rw-rw-rw-   0        0        0     5542 2024-05-25 13:52:47.000000 heflwr-0.1.6/src/heflwr/monitor/process_monitor/prometheus_monitor.py
+-rw-rw-rw-   0        0        0     5350 2024-05-25 13:52:47.000000 heflwr-0.1.6/src/heflwr/monitor/process_monitor/remote_monitor.py
+drwxrwxrwx   0        0        0        0 2024-06-01 12:58:02.123922 heflwr-0.1.6/src/heflwr/monitor/thread_monitor/
+-rw-rw-rw-   0        0        0      133 2024-05-25 11:52:25.000000 heflwr-0.1.6/src/heflwr/monitor/thread_monitor/__init__.py
+-rw-rw-rw-   0        0        0     4939 2024-05-25 13:52:47.000000 heflwr-0.1.6/src/heflwr/monitor/thread_monitor/file_monitor.py
+-rw-rw-rw-   0        0        0     5300 2024-05-25 13:52:47.000000 heflwr-0.1.6/src/heflwr/monitor/thread_monitor/prometheus_monitor.py
+-rw-rw-rw-   0        0        0     5019 2024-05-25 13:52:47.000000 heflwr-0.1.6/src/heflwr/monitor/thread_monitor/remote_monitor.py
+drwxrwxrwx   0        0        0        0 2024-06-01 12:58:02.125915 heflwr-0.1.6/src/heflwr/monitor/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-14 16:05:22.000000 heflwr-0.1.6/src/heflwr/monitor/utils/__init__.py
+-rw-rw-rw-   0        0        0     1028 2024-05-14 16:05:22.000000 heflwr-0.1.6/src/heflwr/monitor/utils/network.py
+-rw-rw-rw-   0        0        0     4500 2024-05-14 16:05:22.000000 heflwr-0.1.6/src/heflwr/monitor/utils/power.py
+drwxrwxrwx   0        0        0        0 2024-06-01 12:58:02.130517 heflwr-0.1.6/src/heflwr/nn/
+-rw-rw-rw-   0        0        0      476 2024-06-01 12:33:13.000000 heflwr-0.1.6/src/heflwr/nn/__init__.py
+-rw-rw-rw-   0        0        0      390 2024-06-01 10:34:00.000000 heflwr-0.1.6/src/heflwr/nn/scaler.py
+-rw-rw-rw-   0        0        0    10162 2024-06-01 11:43:15.000000 heflwr-0.1.6/src/heflwr/nn/ssbatchnorm2d.py
+-rw-rw-rw-   0        0        0     9399 2024-06-01 11:47:08.000000 heflwr-0.1.6/src/heflwr/nn/ssconv2d.py
+-rw-rw-rw-   0        0        0     8985 2024-06-01 11:47:08.000000 heflwr-0.1.6/src/heflwr/nn/sslinear.py
+-rw-rw-rw-   0        0        0      311 2024-06-01 10:26:02.000000 heflwr-0.1.6/src/heflwr/nn/utils.py
+drwxrwxrwx   0        0        0        0 2024-06-01 12:58:02.111943 heflwr-0.1.6/src/heflwr.egg-info/
+-rw-rw-rw-   0        0        0      495 2024-06-01 12:58:01.000000 heflwr-0.1.6/src/heflwr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1160 2024-06-01 12:58:02.000000 heflwr-0.1.6/src/heflwr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 12:58:01.000000 heflwr-0.1.6/src/heflwr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-06-01 12:58:01.000000 heflwr-0.1.6/src/heflwr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 12:58:02.130517 heflwr-0.1.6/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-14 16:05:22.000000 heflwr-0.1.6/tests/test.py
```

### Comparing `heflwr-0.1.5/LICENSE` & `heflwr-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `heflwr-0.1.5/setup.py` & `heflwr-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open("README.rst", encoding="UTF-8") as f:
         return f.read()
 
 
 setup(
     name="heflwr",
-    version="0.1.5",
+    version="0.1.6",
     description="「HeFlwr」is a federated learning package for heterogeneous devices.",
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     author="Zhu Yaolin",
     author_email="zhuyaolinluck@qq.com",
     long_description=readme(),
     long_description_content_type='text/x-rst',
```

### Comparing `heflwr-0.1.5/src/heflwr/fed/aggregate.py` & `heflwr-0.1.6/src/heflwr/fed/aggregate.py`

 * *Files identical despite different names*

### Comparing `heflwr-0.1.5/src/heflwr/fed/heflwr_aggregate.py` & `heflwr-0.1.6/src/heflwr/fed/heflwr_aggregate.py`

 * *Files identical despite different names*

### Comparing `heflwr-0.1.5/src/heflwr/log/configurator.py` & `heflwr-0.1.6/src/heflwr/log/configurator.py`

 * *Files identical despite different names*

### Comparing `heflwr-0.1.5/src/heflwr/log/handlers.py` & `heflwr-0.1.6/src/heflwr/log/handlers.py`

 * *Files identical despite different names*

### Comparing `heflwr-0.1.5/src/heflwr/log/log_info.py` & `heflwr-0.1.6/src/heflwr/log/log_info.py`

 * *Files identical despite different names*

### Comparing `heflwr-0.1.5/src/heflwr/monitor/process_monitor/file_monitor.py` & `heflwr-0.1.6/src/heflwr/monitor/process_monitor/file_monitor.py`

 * *Files identical despite different names*

### Comparing `heflwr-0.1.5/src/heflwr/monitor/process_monitor/prometheus_monitor.py` & `heflwr-0.1.6/src/heflwr/monitor/process_monitor/prometheus_monitor.py`

 * *Files identical despite different names*

### Comparing `heflwr-0.1.5/src/heflwr/monitor/process_monitor/remote_monitor.py` & `heflwr-0.1.6/src/heflwr/monitor/process_monitor/remote_monitor.py`

 * *Files identical despite different names*

### Comparing `heflwr-0.1.5/src/heflwr/monitor/thread_monitor/file_monitor.py` & `heflwr-0.1.6/src/heflwr/monitor/thread_monitor/file_monitor.py`

 * *Files identical despite different names*

### Comparing `heflwr-0.1.5/src/heflwr/monitor/thread_monitor/prometheus_monitor.py` & `heflwr-0.1.6/src/heflwr/monitor/thread_monitor/prometheus_monitor.py`

 * *Files identical despite different names*

### Comparing `heflwr-0.1.5/src/heflwr/monitor/thread_monitor/remote_monitor.py` & `heflwr-0.1.6/src/heflwr/monitor/thread_monitor/remote_monitor.py`

 * *Files identical despite different names*

### Comparing `heflwr-0.1.5/src/heflwr/monitor/utils/network.py` & `heflwr-0.1.6/src/heflwr/monitor/utils/network.py`

 * *Files identical despite different names*

### Comparing `heflwr-0.1.5/src/heflwr/monitor/utils/power.py` & `heflwr-0.1.6/src/heflwr/monitor/utils/power.py`

 * *Files identical despite different names*

### Comparing `heflwr-0.1.5/src/heflwr/nn/ssconv2d.py` & `heflwr-0.1.6/src/heflwr/nn/ssconv2d.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,20 +2,15 @@
 from typing_extensions import Self
 from fractions import Fraction
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
-
-# For example, (0, 0.5) represents extracting the first 50%.
-Interval = Tuple[str, str]
-# For example, [(0, 0.2), (0.5, 0.8)] also represents extracting 50%, but at different positions.
-Intervals = List[Tuple[str, str]]
-Layer_Range = Union[Interval, Intervals]
+from utils import Layer_Range
 
 
 class SSConv2d(nn.Conv2d):
     def __init__(self: Self, in_channels: int, out_channels: int, kernel_size: Union[int, Tuple[int, int]],
                  stride: Union[int, Tuple[int, int]] = 1, padding: Union[int, Tuple[int, int]] = 0,
                  dilation: Union[int, Tuple[int, int]] = 1, groups: int = 1, bias: bool = True,
                  in_channels_ranges: Layer_Range = ('0', '1'), out_channels_ranges: Layer_Range = ('0', '1')) -> None:
@@ -115,53 +110,53 @@
             ret_start = offset
             ret_end = offset + (end - start)
             ret_indices.append((ret_start, ret_end))
             offset = ret_end
         return ret_indices
 
     @staticmethod
-    def get_subset_parameters(father_layer: nn.Conv2d, out_index: List[Tuple[int, int]],
-                              in_index: List[Tuple[int, int]]) -> Tuple[torch.Tensor, Optional[torch.Tensor]]:
+    def get_subset_parameters(father_layer: nn.Conv2d, out_index: Tuple[int, int],
+                              in_index: Tuple[int, int]) -> Tuple[torch.Tensor, Optional[torch.Tensor]]:
         """
         Retrieves the parameters of a subset of the model's weights and biases.
 
         This method is used to get a specific block of the model's weight matrix and the corresponding bias vector.
         It is particularly useful when dealing with layers of models that need to be
         partially extracted based on certain indices.
 
         :param father_layer: The nn.Conv2d layer of the model from which the parameters are to be extracted.
-        :param out_index: A list of tuples specifying the start and end indices
+        :param out_index: A tuple specifying the start and end index
         for the rows in the weight matrix to be retrieved.
-        :param in_index: A list of tuples specifying the start and end indices
+        :param in_index: A tuple specifying the start and end index
         for the columns in the weight matrix to be retrieved.
 
         :return: A tuple containing the extracted weight tensor and bias tensor.
         The bias tensor would be None if the original layer does not have a bias.
         """
         weight = father_layer.weight[out_index[0]: out_index[1], in_index[0]: in_index[1]].clone()
         bias = None
         if father_layer.bias is not None:
             bias = father_layer.bias[out_index[0]: out_index[1]].clone()
         return weight, bias
 
     def set_subset_parameters(self: Self, weight: torch.Tensor, bias: torch.Tensor,
-                              out_index: List[Tuple[int, int]], in_index: List[Tuple[int, int]]) -> None:
+                              out_index: Tuple[int, int], in_index: Tuple[int, int]) -> None:
         """
         Sets the parameters of a subset of the model's weights and biases.
 
         This method is used to update a specific block of the model's weight matrix and the corresponding bias vector.
         It is particularly useful when dealing with layers of models that need to be
         partially updated based on certain indices.
 
         :param weight: A torch.Tensor containing the weight values to be set in the specified subset.
         :param bias: A torch.Tensor containing the bias values to be set in the specified subset.
         If `None`, the bias will not be updated.
-        :param out_index: A list of tuples specifying the start and end indices
+        :param out_index: A tuple specifying the start and end index
         for the rows in the weight matrix to be updated.
-        :param in_index: A list of tuples specifying the start and end indices
+        :param in_index: A tuple specifying the start and end index
         for the columns in the weight matrix to be updated.
 
         :return: None. The method updates the weight and bias in-place.
         """
         self.weight[out_index[0]: out_index[1], in_index[0]: in_index[1]] = weight
         if bias is not None:
             self.bias[out_index[0]: out_index[1]] = bias
```

### Comparing `heflwr-0.1.5/src/heflwr/nn/sslinear.py` & `heflwr-0.1.6/src/heflwr/nn/sslinear.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,28 +2,23 @@
 from typing_extensions import Self
 from fractions import Fraction
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
-
-# For example, (0, 0.5) represents extracting the first 50%.
-Interval = Tuple[str, str]
-# For example, [(0, 0.2), (0.5, 0.8)] also represents extracting 50%, but at different positions.
-Intervals = List[Tuple[str, str]]
-Layer_Range = Union[Interval, Intervals]
+from utils import Layer_Range
 
 
 class SSLinear(nn.Linear):
     def __init__(self: Self, in_features: int, out_features: int, bias: bool = True,
                  in_features_ranges: Layer_Range = ('0', '1'),
                  out_features_ranges: Layer_Range = ('0', '1')) -> None:
 
-        # if in_channels_ranges/out_channels_ranges belong to Interval, then convert into Intervals.
+        # if in_features_ranges/out_features_ranges belong to Interval, then convert into Intervals.
         if isinstance(in_features_ranges[0], str):
             in_features_ranges = [in_features_ranges]
         if isinstance(out_features_ranges[0], str):
             out_features_ranges = [out_features_ranges]
 
         # Convert string interval into fraction interval.
         in_features_ranges = [tuple(map(self.parse_fraction_strings, range_str)) for range_str in in_features_ranges]
@@ -55,15 +50,15 @@
         This method is used to propagate parameters from a parent layer to the current layer, effectively
         initializing or updating the current layer's parameters.
 
         The method identifies matching blocks of parameters between the layers based on their relative
         positions, and uses the `get_subset_parameters` and `set_subset_parameters` methods to transfer
         the parameters.
 
-        :param father_layer: The parent layer of type Self or nn.Conv2d from which the parameters are to be propagated.
+        :param father_layer: The parent layer of type Self or nn.Linear from which the parameters are to be propagated.
 
         :return: None. The method updates the parameters of the current layer in place.
         """
         father_out_indices_start = [int(out_range[0] * father_layer.out_features)
                                     for out_range in self.out_features_ranges]
         father_out_indices_end = [int(out_range[1] * father_layer.out_features)
                                   for out_range in self.out_features_ranges]
@@ -109,53 +104,53 @@
             ret_start = offset
             ret_end = offset + (end - start)
             ret_indices.append((ret_start, ret_end))
             offset = ret_end
         return ret_indices
 
     @staticmethod
-    def get_subset_parameters(father_layer: nn.Linear, out_index: List[Tuple[int, int]],
-                              in_index: List[Tuple[int, int]]) -> Tuple[torch.Tensor, Optional[torch.Tensor]]:
+    def get_subset_parameters(father_layer: nn.Linear, out_index: Tuple[int, int],
+                              in_index: Tuple[int, int]) -> Tuple[torch.Tensor, Optional[torch.Tensor]]:
         """
         Retrieves the parameters of a subset of the model's weights and biases.
 
         This method is used to get a specific block of the model's weight matrix and the corresponding bias vector.
         It is particularly useful when dealing with layers of models that need to be
         partially extracted based on certain indices.
 
-        :param father_layer: The nn.Conv2d layer of the model from which the parameters are to be extracted.
-        :param out_index: A list of tuples specifying the start and end indices
+        :param father_layer: The nn.Linear layer of the model from which the parameters are to be extracted.
+        :param out_index: A tuple specifying the start and end index
         for the rows in the weight matrix to be retrieved.
-        :param in_index: A list of tuples specifying the start and end indices
+        :param in_index: A tuple specifying the start and end index
         for the columns in the weight matrix to be retrieved.
 
         :return: A tuple containing the extracted weight tensor and bias tensor.
         The bias tensor would be None if the original layer does not have a bias.
         """
         weight = father_layer.weight[out_index[0]: out_index[1], in_index[0]: in_index[1]].clone()
         bias = None
         if father_layer.bias is not None:
             bias = father_layer.bias[out_index[0]: out_index[1]].clone()
         return weight, bias
 
     def set_subset_parameters(self: Self, weight: torch.Tensor, bias: torch.Tensor,
-                              out_index: List[Tuple[int, int]], in_index: List[Tuple[int, int]]) -> None:
+                              out_index: Tuple[int, int], in_index: Tuple[int, int]) -> None:
         """
         Sets the parameters of a subset of the model's weights and biases.
 
         This method is used to update a specific block of the model's weight matrix and the corresponding bias vector.
         It is particularly useful when dealing with layers of models that need to be
         partially updated based on certain indices.
 
         :param weight: A torch.Tensor containing the weight values to be set in the specified subset.
         :param bias: A torch.Tensor containing the bias values to be set in the specified subset.
         If `None`, the bias will not be updated.
-        :param out_index: A list of tuples specifying the start and end indices
+        :param out_index: A tuple specifying the start and end index
         for the rows in the weight matrix to be updated.
-        :param in_index: A list of tuples specifying the start and end indices
+        :param in_index: A tuple specifying the start and end index
         for the columns in the weight matrix to be updated.
 
         :return: None. The method updates the weight and bias in-place.
         """
         self.weight[out_index[0]: out_index[1], in_index[0]: in_index[1]] = weight
         if bias is not None:
             self.bias[out_index[0]: out_index[1]] = bias
@@ -174,8 +169,7 @@
         """
         if fraction_str == '0':
             return Fraction(0, 1)
         if fraction_str == '1':
             return Fraction(1, 1)
         numerator, denominator = map(int, fraction_str.split('/'))
         return Fraction(numerator, denominator)
-
```

### Comparing `heflwr-0.1.5/src/heflwr.egg-info/SOURCES.txt` & `heflwr-0.1.6/src/heflwr.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -28,8 +28,9 @@
 src/heflwr/monitor/utils/network.py
 src/heflwr/monitor/utils/power.py
 src/heflwr/nn/__init__.py
 src/heflwr/nn/scaler.py
 src/heflwr/nn/ssbatchnorm2d.py
 src/heflwr/nn/ssconv2d.py
 src/heflwr/nn/sslinear.py
+src/heflwr/nn/utils.py
 tests/test.py
```

