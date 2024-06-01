# Comparing `tmp/ultralytics_thop-0.2.4.tar.gz` & `tmp/ultralytics_thop-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultralytics_thop-0.2.4.tar", last modified: Fri May 31 20:26:57 2024, max compression
+gzip compressed data, was "ultralytics_thop-0.2.5.tar", last modified: Sat Jun  1 01:43:27 2024, max compression
```

## Comparing `ultralytics_thop-0.2.4.tar` & `ultralytics_thop-0.2.5.tar`

### file list

```diff
@@ -1,30 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:26:57.605087 ultralytics_thop-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-31 20:25:56.000000 ultralytics_thop-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-05-31 20:26:57.601087 ultralytics_thop-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-05-31 20:25:56.000000 ultralytics_thop-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-05-31 20:25:56.000000 ultralytics_thop-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 20:26:57.605087 ultralytics_thop-0.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:26:57.601087 ultralytics_thop-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-31 20:25:56.000000 ultralytics_thop-0.2.4/tests/test_conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-31 20:25:56.000000 ultralytics_thop-0.2.4/tests/test_matmul.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-31 20:25:56.000000 ultralytics_thop-0.2.4/tests/test_relu.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-31 20:25:56.000000 ultralytics_thop-0.2.4/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:26:57.601087 ultralytics_thop-0.2.4/thop/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-31 20:25:56.000000 ultralytics_thop-0.2.4/thop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8360 2024-05-31 20:25:56.000000 ultralytics_thop-0.2.4/thop/fx_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-31 20:25:56.000000 ultralytics_thop-0.2.4/thop/onnx_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     7965 2024-05-31 20:25:56.000000 ultralytics_thop-0.2.4/thop/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     6581 2024-05-31 20:25:56.000000 ultralytics_thop-0.2.4/thop/rnn_hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-31 20:25:56.000000 ultralytics_thop-0.2.4/thop/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:26:57.601087 ultralytics_thop-0.2.4/thop/vision/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 20:25:56.000000 ultralytics_thop-0.2.4/thop/vision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-31 20:25:56.000000 ultralytics_thop-0.2.4/thop/vision/basic_hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-05-31 20:25:56.000000 ultralytics_thop-0.2.4/thop/vision/calc_func.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-31 20:25:56.000000 ultralytics_thop-0.2.4/thop/vision/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    13298 2024-05-31 20:25:56.000000 ultralytics_thop-0.2.4/thop/vision/onnx_counter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:26:57.601087 ultralytics_thop-0.2.4/ultralytics_thop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-05-31 20:26:57.000000 ultralytics_thop-0.2.4/ultralytics_thop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-31 20:26:57.000000 ultralytics_thop-0.2.4/ultralytics_thop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 20:26:57.000000 ultralytics_thop-0.2.4/ultralytics_thop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-31 20:26:57.000000 ultralytics_thop-0.2.4/ultralytics_thop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-31 20:26:57.000000 ultralytics_thop-0.2.4/ultralytics_thop.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:43:27.721440 ultralytics_thop-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-06-01 01:42:20.000000 ultralytics_thop-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-06-01 01:43:27.721440 ultralytics_thop-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-06-01 01:42:20.000000 ultralytics_thop-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-06-01 01:42:20.000000 ultralytics_thop-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 01:43:27.721440 ultralytics_thop-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:43:27.721440 ultralytics_thop-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-06-01 01:42:20.000000 ultralytics_thop-0.2.5/tests/test_conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-06-01 01:42:20.000000 ultralytics_thop-0.2.5/tests/test_matmul.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-06-01 01:42:20.000000 ultralytics_thop-0.2.5/tests/test_relu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-06-01 01:42:20.000000 ultralytics_thop-0.2.5/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:43:27.721440 ultralytics_thop-0.2.5/thop/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-06-01 01:42:20.000000 ultralytics_thop-0.2.5/thop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8270 2024-06-01 01:42:20.000000 ultralytics_thop-0.2.5/thop/fx_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7848 2024-06-01 01:42:20.000000 ultralytics_thop-0.2.5/thop/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6485 2024-06-01 01:42:20.000000 ultralytics_thop-0.2.5/thop/rnn_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-06-01 01:42:20.000000 ultralytics_thop-0.2.5/thop/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:43:27.721440 ultralytics_thop-0.2.5/thop/vision/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 01:42:20.000000 ultralytics_thop-0.2.5/thop/vision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-06-01 01:42:20.000000 ultralytics_thop-0.2.5/thop/vision/basic_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-06-01 01:42:20.000000 ultralytics_thop-0.2.5/thop/vision/calc_func.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:43:27.721440 ultralytics_thop-0.2.5/ultralytics_thop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-06-01 01:43:27.000000 ultralytics_thop-0.2.5/ultralytics_thop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-06-01 01:43:27.000000 ultralytics_thop-0.2.5/ultralytics_thop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 01:43:27.000000 ultralytics_thop-0.2.5/ultralytics_thop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-06-01 01:43:27.000000 ultralytics_thop-0.2.5/ultralytics_thop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-06-01 01:43:27.000000 ultralytics_thop-0.2.5/ultralytics_thop.egg-info/top_level.txt
```

### Comparing `ultralytics_thop-0.2.4/LICENSE` & `ultralytics_thop-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ultralytics_thop-0.2.4/PKG-INFO` & `ultralytics_thop-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultralytics-thop
-Version: 0.2.4
+Version: 0.2.5
 Summary: Ultralytics THOP package for fast computation of PyTorch model FLOPs and parameters.
 Author-email: Ligeng Zhu <ligeng.zhu+github@gmail.com>
 Maintainer: Glenn Jocher
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/ultralytics/thop/issues
 Project-URL: Funding, https://ultralytics.com
 Project-URL: Source, https://github.com/ultralytics/thop/
```

### Comparing `ultralytics_thop-0.2.4/README.md` & `ultralytics_thop-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `ultralytics_thop-0.2.4/pyproject.toml` & `ultralytics_thop-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ultralytics_thop-0.2.4/tests/test_conv2d.py` & `ultralytics_thop-0.2.5/tests/test_conv2d.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-import pytest
 import torch
 import torch.nn as nn
-from jinja2 import StrictUndefined
 
 from thop import profile
 
 
 class TestUtils:
     def test_conv2d_no_bias(self):
         """Tests a 2D convolutional layer without bias using THOP profiling with predefined input dimensions and
@@ -18,34 +16,34 @@
         net = nn.Conv2d(in_c, out_c, kernel_size=(kh, kw), stride=s, padding=p, dilation=d, groups=g, bias=False)
         data = torch.randn(n, in_c, ih, iw)
         out = net(data)
 
         _, _, oh, ow = out.shape
 
         flops, params = profile(net, inputs=(data,))
-        assert flops == 810000, f"{flops} v.s. {810000}"
+        assert flops == 810000, f"{flops} v.s. 810000"
 
     def test_conv2d(self):
         """Tests a Conv2D layer with specific input dimensions, kernel size, stride, padding, dilation, and groups."""
         n, in_c, ih, iw = 1, 3, 32, 32  # torch.randint(1, 10, (4,)).tolist()
         out_c, kh, kw = 12, 5, 5
         s, p, d, g = 1, 1, 1, 1
 
         net = nn.Conv2d(in_c, out_c, kernel_size=(kh, kw), stride=s, padding=p, dilation=d, groups=g, bias=True)
         data = torch.randn(n, in_c, ih, iw)
         out = net(data)
 
         _, _, oh, ow = out.shape
 
         flops, params = profile(net, inputs=(data,))
-        assert flops == 810000, f"{flops} v.s. {810000}"
+        assert flops == 810000, f"{flops} v.s. 810000"
 
     def test_conv2d_random(self):
         """Test Conv2D layer with random parameters and validate the computed FLOPs and parameters using 'profile'."""
-        for i in range(10):
+        for _ in range(10):
             out_c, kh, kw = torch.randint(1, 20, (3,)).tolist()
             n, in_c, ih, iw = torch.randint(1, 20, (4,)).tolist()  # torch.randint(1, 10, (4,)).tolist()
             ih += kh
             iw += kw
             s, p, d, g = 1, 1, 1, 1
 
             net = nn.Conv2d(in_c, out_c, kernel_size=(kh, kw), stride=s, padding=p, dilation=d, groups=g, bias=False)
```

### Comparing `ultralytics_thop-0.2.4/tests/test_matmul.py` & `ultralytics_thop-0.2.5/tests/test_matmul.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import pytest
 import torch
 import torch.nn as nn
 
 from thop import profile
 
 
 class TestUtils:
```

### Comparing `ultralytics_thop-0.2.4/tests/test_utils.py` & `ultralytics_thop-0.2.5/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import pytest
-
 from thop import utils
 
 
 class TestUtils:
     def test_clever_format_returns_formatted_number(self):
         """Tests that the clever_format function returns a formatted number string with a '1.00B' pattern."""
         nums = 1
```

### Comparing `ultralytics_thop-0.2.4/thop/fx_profile.py` & `ultralytics_thop-0.2.5/thop/fx_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,17 +81,15 @@
     return int(total_ops)
 
 
 def count_nn_bn2d(module: nn.BatchNorm2d, input_shapes, output_shapes):
     """Calculate the total operations for a given nn.BatchNorm2d module based on its output shape."""
     assert len(output_shapes) == 1, "nn.BatchNorm2d should only have one output"
     y = output_shapes[0]
-    # y = (x - mean) / \sqrt{var + e} * weight + bias
-    total_ops = 2 * y.numel()
-    return total_ops
+    return 2 * y.numel()
 
 
 zero_ops = (
     nn.ReLU,
     nn.ReLU6,
     nn.Dropout,
     nn.MaxPool2d,
@@ -116,15 +114,15 @@
     count_map[k] = count_zero_ops
 
 missing_maps = {}
 
 from torch.fx import symbolic_trace
 from torch.fx.passes.shape_prop import ShapeProp
 
-from .utils import prGreen, prRed, prYellow
+from .utils import prRed, prYellow
 
 
 def null_print(*args, **kwargs):
     """A no-op print function that takes any arguments without performing any actions."""
     return
 
 
@@ -189,15 +187,15 @@
             if type(m) in count_map:
                 node_flops = count_map[type(m)](m, input_shapes, output_shapes)
             else:
                 missing_maps[key] = (node.op,)
                 prRed(f"{key} is missing")
             print("module type:", type(m))
             if isinstance(m, zero_ops):
-                print(f"weight_shape: None")
+                print("weight_shape: None")
             else:
                 print(type(m))
                 print(f"weight_shape: {mod.state_dict()[node.target + '.weight'].shape}")
 
         v_maps[str(node.name)] = node.meta["tensor_meta"].shape
         if node_flops is not None:
             total_flops += node_flops
```

### Comparing `ultralytics_thop-0.2.4/thop/profile.py` & `ultralytics_thop-0.2.5/thop/profile.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from thop.rnn_hooks import *
 from thop.vision.basic_hooks import *
 
-# logger = logging.getLogger(__name__)
-# logger.setLevel(logging.INFO)
-from .utils import prGreen, prRed, prYellow
+from .utils import prRed
 
 default_dtype = torch.float64
 
 register_hooks = {
     nn.ZeroPad2d: zero_ops,  # padding does not involve any multiplication.
     nn.Conv1d: count_convNd,
     nn.Conv2d: count_convNd,
@@ -64,15 +62,15 @@
     types_collection = set()
     if custom_ops is None:
         custom_ops = {}
     if report_missing:
         verbose = True
 
     def add_hooks(m):
-        if len(list(m.children())) > 0:
+        if list(m.children()):
             return
 
         if hasattr(m, "total_ops") or hasattr(m, "total_params"):
             logging.warning(
                 "Either .total_ops or .total_params is already defined in %s. "
                 "Be careful, it might change your code's behavior." % str(m)
             )
@@ -110,30 +108,30 @@
 
     with torch.no_grad():
         model(*inputs)
 
     total_ops = 0
     total_params = 0
     for m in model.modules():
-        if len(list(m.children())) > 0:  # skip for non-leaf module
+        if list(m.children()):  # skip for non-leaf module
             continue
         total_ops += m.total_ops
         total_params += m.total_params
 
     total_ops = total_ops.item()
     total_params = total_params.item()
 
     # reset model to original status
     model.train(training)
     for handler in handler_collection:
         handler.remove()
 
     # remove temporal buffers
     for n, m in model.named_modules():
-        if len(list(m.children())) > 0:
+        if list(m.children()):
             continue
         if "total_ops" in m._buffers:
             m._buffers.pop("total_ops")
         if "total_params" in m._buffers:
             m._buffers.pop("total_params")
 
     return total_ops, total_params
```

### Comparing `ultralytics_thop-0.2.4/thop/rnn_hooks.py` & `ultralytics_thop-0.2.5/thop/rnn_hooks.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,34 +99,33 @@
     input_size = m.input_size
     hidden_size = m.hidden_size
     num_layers = m.num_layers
 
     if isinstance(x[0], PackedSequence):
         batch_size = torch.max(x[0].batch_sizes)
         num_steps = x[0].batch_sizes.size(0)
+    elif m.batch_first:
+        batch_size = x[0].size(0)
+        num_steps = x[0].size(1)
     else:
-        if m.batch_first:
-            batch_size = x[0].size(0)
-            num_steps = x[0].size(1)
-        else:
-            batch_size = x[0].size(1)
-            num_steps = x[0].size(0)
+        batch_size = x[0].size(1)
+        num_steps = x[0].size(0)
 
     total_ops = 0
     if m.bidirectional:
         total_ops += _count_rnn_cell(input_size, hidden_size, bias) * 2
     else:
         total_ops += _count_rnn_cell(input_size, hidden_size, bias)
 
-    for i in range(num_layers - 1):
-        if m.bidirectional:
-            total_ops += _count_rnn_cell(hidden_size * 2, hidden_size, bias) * 2
-        else:
-            total_ops += _count_rnn_cell(hidden_size, hidden_size, bias)
-
+    for _ in range(num_layers - 1):
+        total_ops += (
+            _count_rnn_cell(hidden_size * 2, hidden_size, bias) * 2
+            if m.bidirectional
+            else _count_rnn_cell(hidden_size, hidden_size, bias)
+        )
     # time unroll
     total_ops *= num_steps
     # batch_size
     total_ops *= batch_size
 
     m.total_ops += torch.DoubleTensor([int(total_ops)])
 
@@ -137,34 +136,33 @@
     input_size = m.input_size
     hidden_size = m.hidden_size
     num_layers = m.num_layers
 
     if isinstance(x[0], PackedSequence):
         batch_size = torch.max(x[0].batch_sizes)
         num_steps = x[0].batch_sizes.size(0)
+    elif m.batch_first:
+        batch_size = x[0].size(0)
+        num_steps = x[0].size(1)
     else:
-        if m.batch_first:
-            batch_size = x[0].size(0)
-            num_steps = x[0].size(1)
-        else:
-            batch_size = x[0].size(1)
-            num_steps = x[0].size(0)
+        batch_size = x[0].size(1)
+        num_steps = x[0].size(0)
 
     total_ops = 0
     if m.bidirectional:
         total_ops += _count_gru_cell(input_size, hidden_size, bias) * 2
     else:
         total_ops += _count_gru_cell(input_size, hidden_size, bias)
 
-    for i in range(num_layers - 1):
-        if m.bidirectional:
-            total_ops += _count_gru_cell(hidden_size * 2, hidden_size, bias) * 2
-        else:
-            total_ops += _count_gru_cell(hidden_size, hidden_size, bias)
-
+    for _ in range(num_layers - 1):
+        total_ops += (
+            _count_gru_cell(hidden_size * 2, hidden_size, bias) * 2
+            if m.bidirectional
+            else _count_gru_cell(hidden_size, hidden_size, bias)
+        )
     # time unroll
     total_ops *= num_steps
     # batch_size
     total_ops *= batch_size
 
     m.total_ops += torch.DoubleTensor([int(total_ops)])
 
@@ -177,33 +175,32 @@
     input_size = m.input_size
     hidden_size = m.hidden_size
     num_layers = m.num_layers
 
     if isinstance(x[0], PackedSequence):
         batch_size = torch.max(x[0].batch_sizes)
         num_steps = x[0].batch_sizes.size(0)
+    elif m.batch_first:
+        batch_size = x[0].size(0)
+        num_steps = x[0].size(1)
     else:
-        if m.batch_first:
-            batch_size = x[0].size(0)
-            num_steps = x[0].size(1)
-        else:
-            batch_size = x[0].size(1)
-            num_steps = x[0].size(0)
+        batch_size = x[0].size(1)
+        num_steps = x[0].size(0)
 
     total_ops = 0
     if m.bidirectional:
         total_ops += _count_lstm_cell(input_size, hidden_size, bias) * 2
     else:
         total_ops += _count_lstm_cell(input_size, hidden_size, bias)
 
-    for i in range(num_layers - 1):
-        if m.bidirectional:
-            total_ops += _count_lstm_cell(hidden_size * 2, hidden_size, bias) * 2
-        else:
-            total_ops += _count_lstm_cell(hidden_size, hidden_size, bias)
-
+    for _ in range(num_layers - 1):
+        total_ops += (
+            _count_lstm_cell(hidden_size * 2, hidden_size, bias) * 2
+            if m.bidirectional
+            else _count_lstm_cell(hidden_size, hidden_size, bias)
+        )
     # time unroll
     total_ops *= num_steps
     # batch_size
     total_ops *= batch_size
 
     m.total_ops += torch.DoubleTensor([int(total_ops)])
```

### Comparing `ultralytics_thop-0.2.4/thop/utils.py` & `ultralytics_thop-0.2.5/thop/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,23 +16,14 @@
     return actual_call
 
 
 prRed = colorful_print(print, color=COLOR_RED)
 prGreen = colorful_print(print, color=COLOR_GREEN)
 prYellow = colorful_print(print, color=COLOR_YELLOW)
 
-# def prRed(skk):
-#     print("\033[91m{}\033[00m".format(skk))
-
-# def prGreen(skk):
-#     print("\033[92m{}\033[00m".format(skk))
-
-# def prYellow(skk):
-#     print("\033[93m{}\033[00m".format(skk))
-
 
 def clever_format(nums, format="%.2f"):
     """Formats numerical values into a more readable string with units (K, M, G, T) based on their magnitude."""
     if not isinstance(nums, Iterable):
         nums = [nums]
     clever_nums = []
 
@@ -44,16 +35,14 @@
         elif num > 1e6:
             clever_nums.append(format % (num / 1e6) + "M")
         elif num > 1e3:
             clever_nums.append(format % (num / 1e3) + "K")
         else:
             clever_nums.append(format % num + "B")
 
-    clever_nums = clever_nums[0] if len(clever_nums) == 1 else (*clever_nums,)
-
-    return clever_nums
+    return clever_nums[0] if len(clever_nums) == 1 else (*clever_nums,)
 
 
 if __name__ == "__main__":
     prRed("hello", "world")
     prGreen("hello", "world")
     prYellow("hello", "world")
```

### Comparing `ultralytics_thop-0.2.4/thop/vision/basic_hooks.py` & `ultralytics_thop-0.2.5/thop/vision/basic_hooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-import argparse
 import logging
 
-import torch
 import torch.nn as nn
 from torch.nn.modules.conv import _ConvNd
 
 from .calc_func import *
 
 multiply_adds = 1
 
@@ -135,15 +133,15 @@
     """Update the total operations counter in the given module for supported upsampling modes."""
     if m.mode not in (
         "nearest",
         "linear",
         "bilinear",
         "bicubic",
     ):  # "trilinear"
-        logging.warning("mode %s is not implemented yet, take it a zero op" % m.mode)
+        logging.warning(f"mode {m.mode} is not implemented yet, take it a zero op")
         m.total_ops += 0
     else:
         x = x[0]
         m.total_ops += calculate_upsample(m.mode, y.nelement())
 
 
 # nn.Linear
```

### Comparing `ultralytics_thop-0.2.4/thop/vision/calc_func.py` & `ultralytics_thop-0.2.5/thop/vision/calc_func.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,31 +10,25 @@
     for _ in in_list:
         res *= _
     return res
 
 
 def l_sum(in_list):
     """Calculate the sum of all elements in a list."""
-    res = 0
-    for _ in in_list:
-        res += _
-    return res
+    return sum(in_list)
 
 
 def calculate_parameters(param_list):
     """Calculate the total number of parameters in a list of tensors."""
-    total_params = 0
-    for p in param_list:
-        total_params += torch.DoubleTensor([p.nelement()])
-    return total_params
+    return sum(torch.DoubleTensor([p.nelement()]) for p in param_list)
 
 
 def calculate_zero_ops():
     """Return a tensor initialized to zero."""
-    return torch.DoubleTensor([int(0)])
+    return torch.DoubleTensor([0])
 
 
 def calculate_conv2d_flops(input_size: list, output_size: list, kernel_size: list, groups: int, bias: bool = False):
     """Calculate FLOPs for a Conv2D layer given input/output sizes, kernel size, groups, and bias flag."""
     # n, in_c, ih, iw = input_size
     # out_c, in_c, kh, kw = kernel_size
     in_c = input_size[1]
@@ -86,22 +80,20 @@
     kernel_op = kernel_size + total_div
     return torch.DoubleTensor([int(kernel_op * output_size)])
 
 
 def calculate_upsample(mode: str, output_size):
     """Calculate the number of operations for upsample methods given the mode and output size."""
     total_ops = output_size
-    if mode == "linear":
-        total_ops *= 5
+    if mode == "bicubic":
+        total_ops *= 224 + 35
     elif mode == "bilinear":
         total_ops *= 11
-    elif mode == "bicubic":
-        ops_solve_A = 224  # 128 muls + 96 adds
-        ops_solve_p = 35  # 16 muls + 12 adds + 4 muls + 3 adds
-        total_ops *= ops_solve_A + ops_solve_p
+    elif mode == "linear":
+        total_ops *= 5
     elif mode == "trilinear":
         total_ops *= 13 * 2 + 5
     return torch.DoubleTensor([int(total_ops)])
 
 
 def calculate_linear(in_feature, num_elements):
     """Calculate the linear operation count for an input feature and number of elements."""
```

### Comparing `ultralytics_thop-0.2.4/ultralytics_thop.egg-info/PKG-INFO` & `ultralytics_thop-0.2.5/ultralytics_thop.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultralytics-thop
-Version: 0.2.4
+Version: 0.2.5
 Summary: Ultralytics THOP package for fast computation of PyTorch model FLOPs and parameters.
 Author-email: Ligeng Zhu <ligeng.zhu+github@gmail.com>
 Maintainer: Glenn Jocher
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/ultralytics/thop/issues
 Project-URL: Funding, https://ultralytics.com
 Project-URL: Source, https://github.com/ultralytics/thop/
```

