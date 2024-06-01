# Comparing `tmp/albucore-0.0.6.tar.gz` & `tmp/albucore-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "albucore-0.0.6.tar", last modified: Wed May 29 21:29:30 2024, max compression
+gzip compressed data, was "albucore-0.0.7.tar", last modified: Sat Jun  1 00:42:21 2024, max compression
```

## Comparing `albucore-0.0.6.tar` & `albucore-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 vladimiriglovikov   (501) staff       (20)        0 2024-05-29 21:29:30.521673 albucore-0.0.6/
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     1075 2024-05-14 02:01:45.000000 albucore-0.0.6/LICENSE
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     3059 2024-05-29 21:29:30.521488 albucore-0.0.6/PKG-INFO
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     1349 2024-05-29 02:05:51.000000 albucore-0.0.6/README.md
-drwxr-xr-x   0 vladimiriglovikov   (501) staff       (20)        0 2024-05-29 21:29:30.519453 albucore-0.0.6/albucore/
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)       48 2024-05-29 21:29:24.000000 albucore-0.0.6/albucore/__init__.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     7030 2024-05-29 21:29:24.000000 albucore-0.0.6/albucore/functions.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     6237 2024-05-29 21:29:24.000000 albucore-0.0.6/albucore/utils.py
-drwxr-xr-x   0 vladimiriglovikov   (501) staff       (20)        0 2024-05-29 21:29:30.521281 albucore-0.0.6/albucore.egg-info/
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     3059 2024-05-29 21:29:30.000000 albucore-0.0.6/albucore.egg-info/PKG-INFO
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)      377 2024-05-29 21:29:30.000000 albucore-0.0.6/albucore.egg-info/SOURCES.txt
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)        1 2024-05-29 21:29:30.000000 albucore-0.0.6/albucore.egg-info/dependency_links.txt
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)        1 2024-05-15 02:11:09.000000 albucore-0.0.6/albucore.egg-info/not-zip-safe
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)       60 2024-05-29 21:29:30.000000 albucore-0.0.6/albucore.egg-info/requires.txt
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)        9 2024-05-29 21:29:30.000000 albucore-0.0.6/albucore.egg-info/top_level.txt
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     2611 2024-05-16 02:10:17.000000 albucore-0.0.6/pyproject.toml
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)       38 2024-05-29 21:29:30.521723 albucore-0.0.6/setup.cfg
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     3671 2024-05-28 22:32:30.000000 albucore-0.0.6/setup.py
-drwxr-xr-x   0 vladimiriglovikov   (501) staff       (20)        0 2024-05-29 21:29:30.521114 albucore-0.0.6/tests/
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     8273 2024-05-29 21:29:24.000000 albucore-0.0.6/tests/test_add.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)    10449 2024-05-29 02:05:51.000000 albucore-0.0.6/tests/test_multiply.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     4089 2024-05-29 21:29:24.000000 albucore-0.0.6/tests/test_normalize.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     2207 2024-05-29 21:29:24.000000 albucore-0.0.6/tests/test_utils.py
+drwxr-xr-x   0 vladimiriglovikov   (501) staff       (20)        0 2024-06-01 00:42:21.074038 albucore-0.0.7/
+-rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     1075 2024-05-14 02:01:45.000000 albucore-0.0.7/LICENSE
+-rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     3059 2024-06-01 00:42:21.073832 albucore-0.0.7/PKG-INFO
+-rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     1349 2024-05-29 02:05:51.000000 albucore-0.0.7/README.md
+drwxr-xr-x   0 vladimiriglovikov   (501) staff       (20)        0 2024-06-01 00:42:21.071871 albucore-0.0.7/albucore/
+-rw-r--r--   0 vladimiriglovikov   (501) staff       (20)       48 2024-06-01 00:42:18.000000 albucore-0.0.7/albucore/__init__.py
+-rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     9538 2024-06-01 00:42:18.000000 albucore-0.0.7/albucore/functions.py
+-rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     6237 2024-05-29 21:29:24.000000 albucore-0.0.7/albucore/utils.py
+drwxr-xr-x   0 vladimiriglovikov   (501) staff       (20)        0 2024-06-01 00:42:21.073653 albucore-0.0.7/albucore.egg-info/
+-rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     3059 2024-06-01 00:42:21.000000 albucore-0.0.7/albucore.egg-info/PKG-INFO
+-rw-r--r--   0 vladimiriglovikov   (501) staff       (20)      424 2024-06-01 00:42:21.000000 albucore-0.0.7/albucore.egg-info/SOURCES.txt
+-rw-r--r--   0 vladimiriglovikov   (501) staff       (20)        1 2024-06-01 00:42:21.000000 albucore-0.0.7/albucore.egg-info/dependency_links.txt
+-rw-r--r--   0 vladimiriglovikov   (501) staff       (20)        1 2024-05-15 02:11:09.000000 albucore-0.0.7/albucore.egg-info/not-zip-safe
+-rw-r--r--   0 vladimiriglovikov   (501) staff       (20)       60 2024-06-01 00:42:21.000000 albucore-0.0.7/albucore.egg-info/requires.txt
+-rw-r--r--   0 vladimiriglovikov   (501) staff       (20)        9 2024-06-01 00:42:21.000000 albucore-0.0.7/albucore.egg-info/top_level.txt
+-rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     2611 2024-05-16 02:10:17.000000 albucore-0.0.7/pyproject.toml
+-rw-r--r--   0 vladimiriglovikov   (501) staff       (20)       38 2024-06-01 00:42:21.074073 albucore-0.0.7/setup.cfg
+-rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     3671 2024-05-28 22:32:30.000000 albucore-0.0.7/setup.py
+drwxr-xr-x   0 vladimiriglovikov   (501) staff       (20)        0 2024-06-01 00:42:21.073509 albucore-0.0.7/tests/
+-rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     7747 2024-06-01 00:42:18.000000 albucore-0.0.7/tests/test_add.py
+-rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     4971 2024-06-01 00:42:18.000000 albucore-0.0.7/tests/test_add_weighted.py
+-rw-r--r--   0 vladimiriglovikov   (501) staff       (20)    10475 2024-06-01 00:42:18.000000 albucore-0.0.7/tests/test_multiply.py
+-rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     4190 2024-05-31 18:36:42.000000 albucore-0.0.7/tests/test_normalize.py
+-rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     4824 2024-06-01 00:42:18.000000 albucore-0.0.7/tests/test_power.py
+-rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     2207 2024-05-29 21:29:24.000000 albucore-0.0.7/tests/test_utils.py
```

### Comparing `albucore-0.0.6/LICENSE` & `albucore-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `albucore-0.0.6/PKG-INFO` & `albucore-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: albucore
-Version: 0.0.6
+Version: 0.0.7
 Summary: A high-performance image processing library designed to optimize and extend the Albumentations library with specialized functions for advanced image transformations. Perfect for developers working in computer vision who require efficient and scalable image augmentation.
 Home-page: https://github.com/albumentations-team/albucore
 Author: Vladimir I. Iglovikov
 License: MIT
 Keywords: Image Processing,Computer Vision,Image Augmentation,Albumentations,Optimization,Machine Learning,Deep Learning,Python Imaging,Data Augmentation,Performance,Efficiency,High-Performance,CV,OpenCV,Automation
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `albucore-0.0.6/README.md` & `albucore-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `albucore-0.0.6/albucore/functions.py` & `albucore-0.0.7/albucore/functions.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     convert_value,
     get_num_channels,
     preserve_channel_dim,
 )
 
 
 @preserve_channel_dim
-def multiply_with_lut(img: np.ndarray, value: Union[Sequence[float], float]) -> np.ndarray:
+def multiply_lut(img: np.ndarray, value: Union[Sequence[float], float]) -> np.ndarray:
     dtype = img.dtype
     max_value = MAX_VALUES_BY_DTYPE[dtype]
 
     if isinstance(value, (int, float)):
         lut = clip(np.arange(0, max_value + 1, dtype=np.float32) * value, dtype)
         return cv2.LUT(img, lut)
 
@@ -30,45 +30,43 @@
     luts = clip(np.arange(0, max_value + 1, dtype=np.float32) * value, dtype)
 
     images = [cv2.LUT(img[:, :, i], luts[i]) for i in range(num_channels)]
     return np.stack(images, axis=-1)
 
 
 @preserve_channel_dim
-@clipped
-def multiply_with_opencv(img: np.ndarray, value: Union[np.ndarray, float]) -> np.ndarray:
+def multiply_opencv(img: np.ndarray, value: Union[np.ndarray, float]) -> np.ndarray:
     return cv2.multiply(img.astype(np.float32), value, dtype=cv2.CV_64F)
 
 
-@clipped
-def multiply_with_numpy(img: np.ndarray, value: Union[float, np.ndarray]) -> np.ndarray:
+def multiply_numpy(img: np.ndarray, value: Union[float, np.ndarray]) -> np.ndarray:
     return np.multiply(img, value)
 
 
 def multiply_by_constant(img: np.ndarray, value: float) -> np.ndarray:
     if img.dtype == np.uint8:
-        return multiply_with_lut(img, value)
+        return multiply_lut(img, value)
     if img.dtype == np.float32:
-        return multiply_with_numpy(img, value)
-    return multiply_with_opencv(img, value)
+        return multiply_numpy(img, value)
+    return multiply_opencv(img, value)
 
 
 def multiply_by_vector(img: np.ndarray, value: np.ndarray) -> np.ndarray:
     num_channels = get_num_channels(img)
     # Handle uint8 images separately to use a lookup table for performance
     if img.dtype == np.uint8:
-        return multiply_with_lut(img, value)
+        return multiply_lut(img, value)
     # Check if the number of channels exceeds the maximum that OpenCV can handle
     if num_channels > MAX_OPENCV_WORKING_CHANNELS:
-        return multiply_with_numpy(img, value)
-    return multiply_with_opencv(img, value)
+        return multiply_numpy(img, value)
+    return multiply_opencv(img, value)
 
 
 def multiply_by_array(img: np.ndarray, value: np.ndarray) -> np.ndarray:
-    return multiply_with_numpy(img, value)
+    return multiply_numpy(img, value)
 
 
 @clipped
 def multiply(img: np.ndarray, value: ValueType) -> np.ndarray:
     num_channels = get_num_channels(img)
     value = convert_value(value, num_channels)
 
@@ -78,26 +76,24 @@
     if isinstance(value, np.ndarray) and value.ndim == 1:
         return multiply_by_vector(img, value)
 
     return multiply_by_array(img, value)
 
 
 @preserve_channel_dim
-@clipped
-def add_with_opencv(img: np.ndarray, value: Union[np.ndarray, float]) -> np.ndarray:
+def add_opencv(img: np.ndarray, value: Union[np.ndarray, float]) -> np.ndarray:
     return cv2.add(img.astype(np.float32), value, dtype=cv2.CV_64F)
 
 
-@clipped
-def add_with_numpy(img: np.ndarray, value: Union[float, np.ndarray]) -> np.ndarray:
+def add_numpy(img: np.ndarray, value: Union[float, np.ndarray]) -> np.ndarray:
     return np.add(img.astype(np.float32), value)
 
 
 @preserve_channel_dim
-def add_with_lut(img: np.ndarray, value: Union[Sequence[float], float]) -> np.ndarray:
+def add_lut(img: np.ndarray, value: Union[Sequence[float], float]) -> np.ndarray:
     dtype = img.dtype
     max_value = MAX_VALUES_BY_DTYPE[dtype]
 
     if isinstance(value, (float, int)):
         lut = clip(np.arange(0, max_value + 1, dtype=np.float32) + value, dtype)
         return cv2.LUT(img, lut)
 
@@ -109,35 +105,36 @@
 
     images = [cv2.LUT(img[:, :, i], luts[i]) for i in range(num_channels)]
     return np.stack(images, axis=-1)
 
 
 def add_constant(img: np.ndarray, value: float) -> np.ndarray:
     if img.dtype == np.uint8:
-        return add_with_lut(img, value)
+        return add_lut(img, value)
     if img.dtype == np.float32:
-        return add_with_numpy(img, value)
-    return add_with_opencv(img, value)
+        return add_numpy(img, value)
+    return add_opencv(img, value)
 
 
 def add_vector(img: np.ndarray, value: np.ndarray) -> np.ndarray:
     num_channels = get_num_channels(img)
     # Handle uint8 images separately to use a lookup table for performance
     if img.dtype == np.uint8:
-        return add_with_lut(img, value)
+        return add_lut(img, value)
     # Check if the number of channels exceeds the maximum that OpenCV can handle
     if num_channels > MAX_OPENCV_WORKING_CHANNELS:
-        return add_with_numpy(img, value)
-    return add_with_opencv(img, value)
+        return add_numpy(img, value)
+    return add_opencv(img, value)
 
 
 def add_array(img: np.ndarray, value: np.ndarray) -> np.ndarray:
-    return add_with_numpy(img, value)
+    return add_numpy(img, value)
 
 
+@clipped
 def add(img: np.ndarray, value: ValueType) -> np.ndarray:
     num_channels = get_num_channels(img)
     value = convert_value(value, num_channels)
 
     if isinstance(value, (float, int)):
         if value == 0:
             return img
@@ -204,11 +201,92 @@
 def normalize(img: np.ndarray, mean: ValueType, denominator: ValueType) -> np.ndarray:
     num_channels = get_num_channels(img)
     denominator = convert_value(denominator, num_channels)
     mean = convert_value(mean, num_channels)
     if img.dtype == np.uint8:
         return normalize_lut(img, mean, denominator)
 
-    if num_channels > MAX_OPENCV_WORKING_CHANNELS:
-        return normalize_numpy(img, mean, denominator)
-
     return normalize_opencv(img, mean, denominator)
+
+
+def power_numpy(img: np.ndarray, exponent: Union[float, np.ndarray]) -> np.ndarray:
+    return np.power(img, exponent)
+
+
+@preserve_channel_dim
+def power_opencv(img: np.ndarray, exponent: Union[float, np.ndarray]) -> np.ndarray:
+    return cv2.pow(img.astype(np.float32), exponent)
+
+
+@preserve_channel_dim
+def power_lut(img: np.ndarray, exponent: Union[float, np.ndarray]) -> np.ndarray:
+    dtype = img.dtype
+    max_value = MAX_VALUES_BY_DTYPE[dtype]
+    num_channels = get_num_channels(img)
+
+    if isinstance(exponent, (float, int)):
+        lut = clip(np.power(np.arange(0, max_value + 1, dtype=np.float32), exponent), dtype)
+        return cv2.LUT(img, lut)
+
+    if isinstance(exponent, np.ndarray) and exponent.shape != ():
+        exponent = exponent.reshape(-1, 1)
+
+    luts = clip(np.power(np.arange(0, max_value + 1, dtype=np.float32), exponent), dtype)
+
+    images = [cv2.LUT(img[:, :, i], luts[i]) for i in range(num_channels)]
+    return np.stack(images, axis=-1)
+
+
+@clipped
+def power(img: np.ndarray, exponent: ValueType) -> np.ndarray:
+    num_channels = get_num_channels(img)
+    exponent = convert_value(exponent, num_channels)
+    if img.dtype == np.uint8:
+        return power_lut(img, exponent)
+
+    if isinstance(exponent, (float, int)):
+        return power_opencv(img, exponent)
+
+    return power_numpy(img, exponent)
+
+
+def add_weighted_numpy(img1: np.ndarray, weight1: float, img2: np.ndarray, weight2: float) -> np.ndarray:
+    return img1 * weight1 + img2 * weight2
+
+
+@preserve_channel_dim
+def add_weighted_opencv(img1: np.ndarray, weight1: float, img2: np.ndarray, weight2: float) -> np.ndarray:
+    return cv2.addWeighted(img1.astype(np.float32), weight1, img2.astype(np.float32), weight2, 0)
+
+
+@preserve_channel_dim
+def add_weighted_lut(img1: np.ndarray, weight1: float, img2: np.ndarray, weight2: float) -> np.ndarray:
+    dtype = img1.dtype
+    max_value = MAX_VALUES_BY_DTYPE[dtype]
+
+    if weight1 == 1 and weight2 == 0:
+        return img1
+
+    if weight1 == 0 and weight2 == 1:
+        return img2
+
+    if weight1 == 0 and weight2 == 0:
+        return np.zeros_like(img1)
+
+    if weight1 == 1 and weight2 == 1:
+        return add_array(img1, img2)
+
+    lut1 = np.arange(0, max_value + 1, dtype=np.float32) * weight1
+    result1 = cv2.LUT(img1, lut1)
+
+    lut2 = np.arange(0, max_value + 1, dtype=np.float32) * weight2
+    result2 = cv2.LUT(img2, lut2)
+
+    return add_array(result1, result2)
+
+
+@clipped
+def add_weighted(img1: np.ndarray, weight1: float, img2: np.ndarray, weight2: float) -> np.ndarray:
+    if img1.shape != img2.shape:
+        raise ValueError(f"The input images must have the same shape. Got {img1.shape} and {img2.shape}.")
+
+    return add_weighted_opencv(img1, weight1, img2, weight2)
```

### Comparing `albucore-0.0.6/albucore/utils.py` & `albucore-0.0.7/albucore/utils.py`

 * *Files identical despite different names*

### Comparing `albucore-0.0.6/albucore.egg-info/PKG-INFO` & `albucore-0.0.7/albucore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: albucore
-Version: 0.0.6
+Version: 0.0.7
 Summary: A high-performance image processing library designed to optimize and extend the Albumentations library with specialized functions for advanced image transformations. Perfect for developers working in computer vision who require efficient and scalable image augmentation.
 Home-page: https://github.com/albumentations-team/albucore
 Author: Vladimir I. Iglovikov
 License: MIT
 Keywords: Image Processing,Computer Vision,Image Augmentation,Albumentations,Optimization,Machine Learning,Deep Learning,Python Imaging,Data Augmentation,Performance,Efficiency,High-Performance,CV,OpenCV,Automation
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `albucore-0.0.6/pyproject.toml` & `albucore-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `albucore-0.0.6/setup.py` & `albucore-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `albucore-0.0.6/tests/test_add.py` & `albucore-0.0.7/tests/test_add.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,20 @@
 import pytest
 import numpy as np
 from albucore.utils import MAX_OPENCV_WORKING_CHANNELS, clip
 from albucore import (
-    add_with_lut,
-    add_with_numpy,
-    add_with_opencv,
+    add_lut,
+    add_numpy,
+    add_opencv,
     add,
     convert_value,
 )
 
 
 @pytest.mark.parametrize(
-    "value, num_channels, expected",
-    [
-        ((1.5), 1, 1.5),
-        (np.array([1.5]), 3, 1.5),
-        ([1.5], 2, 1.5),
-        ([1.5, 2.5], 1, 1.5),
-        ([1.5, 2.5, 0.5], 2, np.array([1.5, 2.5,], dtype=np.float32)),
-        ((1.5), 2, 1.5),
-    ]
-)
-def test_convert_multiplier(value, num_channels, expected):
-    result = convert_value(value, num_channels)
-    if isinstance(expected, np.ndarray):
-        assert np.array_equal(result, expected)
-    else:
-         assert result == expected
-
-
-@pytest.mark.parametrize(
     "img, value, expected_output",
     [
         # Test case 1: Value as a float, image of type uint8
         (
             np.array([[[1, 2, 3], [4, 5, 6]], [[7, 8, 9], [10, 11, 12]]], dtype=np.uint8),
             2.0,
             np.array([[[3, 4, 5], [6, 7, 8]], [[9, 10, 11], [12, 13, 14]]], dtype=np.uint8),
@@ -79,19 +60,19 @@
             np.array([[[0.1, 0.2, 0.3], [0.4, 0.5, 0.6]], [[0.7, 0.8, 0.9], [1.0, 1.1, 1.2]]], dtype=np.float32),
             1.0,
             np.array([[[1.0, 1.0, 1.0], [1.0, 1.0, 1.0]], [[1.0, 1.0, 1.0], [1.0, 1.0, 1.0]]], dtype=np.float32),
         ),
     ],
 )
 def test_add_with_numpy(img, value, expected_output):
-    result_numpy = add_with_numpy(img, value)
+    result_numpy = clip(add_numpy(img, value), img.dtype)
     assert np.allclose(result_numpy, expected_output, atol=1e-6)
 
     if img.shape[-1] in {2, 3} and img.dtype == np.uint8:
-        result_opencv = add_with_opencv(img, value)
+        result_opencv = clip(add_opencv(img, value), img.dtype)
         assert np.allclose(result_opencv, expected_output, atol=1e-6)
 
 
 @pytest.mark.parametrize(
     "img, value, expected_output",
     [
         # Test case 1: Value as a float, image of type uint8
@@ -111,15 +92,15 @@
             np.array([[[100, 150, 200], [250, 255, 100]], [[50, 75, 125], [175, 200, 225]]], dtype=np.uint8),
             60,
             np.array([[[160, 210, 255], [255, 255, 160]], [[110, 135, 185], [235, 255, 255]]], dtype=np.uint8),
         ),
     ],
 )
 def test_add_with_lut(img, value, expected_output):
-    result_lut = add_with_lut(img, value)
+    result_lut = add_lut(img, value)
     assert np.allclose(result_lut, expected_output, atol=1e-6)
 
 
 @pytest.mark.parametrize(
     "img_dtype", [np.uint8, np.float32]
 )
 @pytest.mark.parametrize(
@@ -156,27 +137,27 @@
 
     processed_value = convert_value(value, num_channels)
 
     result = add(img, value)
 
     assert np.array_equal(img, original_image), "Input image was modified"
 
-    result_numpy = add_with_numpy(img, processed_value)
+    result_numpy = clip(add_numpy(img, processed_value), img_dtype)
 
     assert np.array_equal(img, original_image), "Input image was modified"
 
     assert np.allclose(result, result_numpy, atol=1e-6)
 
     if num_channels <= MAX_OPENCV_WORKING_CHANNELS and img.dtype == np.uint8:
-        result_lut = clip(add_with_lut(img, processed_value), img.dtype)
+        result_lut = clip(add_lut(img, processed_value), img.dtype)
         assert np.array_equal(img, original_image), "Input image was modified"
         assert np.array_equal(result, result_lut), f"Difference {(result - result_lut).mean()}"
 
     if num_channels <= MAX_OPENCV_WORKING_CHANNELS:
-        result_opencv = clip(add_with_opencv(img, processed_value), img.dtype)
+        result_opencv = clip(add_opencv(img, processed_value), img.dtype)
         assert np.array_equal(img, original_image), "Input image was modified"
 
         assert np.allclose(result, result_opencv, atol=1e-6), f"Difference {(result - result_opencv).max()}"
 
 @pytest.mark.parametrize(
     ["shift_params", "expected"], [[(-10, 0, 10), (117, 127, 137)], [(-200, 0, 200), (0, 127, 255)]]
 )
```

### Comparing `albucore-0.0.6/tests/test_multiply.py` & `albucore-0.0.7/tests/test_multiply.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import pytest
 import numpy as np
 
 
 from albucore.utils import MAX_OPENCV_WORKING_CHANNELS, clip
 
 from albucore import (
-    multiply_with_lut,
-    multiply_with_numpy,
-    multiply_with_opencv,
+    multiply_lut,
+    multiply_numpy,
+    multiply_opencv,
     multiply,
     convert_value,
 )
 
 
 @pytest.mark.parametrize(
     "img, multiplier, expected_output",
@@ -111,19 +111,19 @@
             np.array([[[0.1, 0.2, 0.3, 0.4, 0.5], [0.6, 0.7, 0.8, 0.9, 1.0]], [[1.1, 1.2, 1.3, 1.4, 1.5], [1.6, 1.7, 1.8, 1.9, 2.0]]], dtype=np.float32),
             np.array([0.5, 1.5, 2.0, 2.5, 3.0], dtype=np.float32),
             np.array([[[0.05, 0.3, 0.6, 1.0, 1.0], [0.3, 1.0, 1.0, 1.0, 1.0]], [[0.55, 1.0, 1.0, 1.0, 1.0], [0.8, 1.0, 1.0, 1.0, 1.0]]], dtype=np.float32),
         ),
     ],
 )
 def test_multiply_with_numpy(img, multiplier, expected_output):
-    result_numpy = multiply_with_numpy(img, multiplier)
+    result_numpy = clip(multiply_numpy(img, multiplier), img.dtype)
     assert np.allclose(result_numpy, expected_output, atol=1e-6)
 
-    if img.shape[-1] in {2, 3} and img.dtype == np.uint8:
-        result_opencv = multiply_with_opencv(img, multiplier)
+    if img.shape[-1] in {1, 3, 4} and img.dtype == np.uint8:
+        result_opencv = clip(multiply_opencv(img, multiplier), img.dtype)
         assert np.allclose(result_opencv, expected_output, atol=1e-6)
 
 
 @pytest.mark.parametrize(
     "img, multiplier, expected_output",
     [
         # Test case 1: Multiplier as a float, image of type uint8
@@ -161,15 +161,15 @@
             np.array([[[1], [2]], [[3], [4]]], dtype=np.uint8),
             2.0,
             np.array([[[2], [4]], [[6], [8]]], dtype=np.uint8),
         ),
     ],
 )
 def test_multiply_with_lut(img, multiplier, expected_output):
-    result_lut = multiply_with_lut(img, multiplier)
+    result_lut = clip(multiply_lut(img, multiplier), img.dtype)
     assert np.allclose(result_lut, expected_output, atol=1e-6)
 
 
 np.random.seed(0)
 
 
 @pytest.mark.parametrize("img_dtype", [np.uint8, np.float32])
@@ -203,23 +203,23 @@
 
     processed_multiplier = convert_value(multiplier, num_channels)
 
     result = multiply(img, multiplier)
 
     assert np.array_equal(img, original_image), "Input image was modified"
 
-    result_numpy = multiply_with_numpy(img, processed_multiplier)
+    result_numpy = clip(multiply_numpy(img, processed_multiplier), img.dtype)
 
     assert np.array_equal(img, original_image), "Input image was modified"
 
     assert np.allclose(result, result_numpy, atol=1e-6)
 
     if num_channels <= MAX_OPENCV_WORKING_CHANNELS and img.dtype == np.uint8:
-        result_lut = clip(multiply_with_lut(img, processed_multiplier), img.dtype)
+        result_lut = clip(multiply_lut(img, processed_multiplier), img.dtype)
         assert np.array_equal(img, original_image), "Input image was modified"
         assert np.array_equal(result, result_lut), f"Difference {(result - result_lut).mean()}"
 
     if num_channels <= MAX_OPENCV_WORKING_CHANNELS:
-        result_opencv = clip(multiply_with_opencv(img, processed_multiplier), img.dtype)
+        result_opencv = clip(multiply_opencv(img, processed_multiplier), img.dtype)
         assert np.array_equal(img, original_image), "Input image was modified"
 
         assert np.allclose(result, result_opencv, atol=1e-6), f"Difference {(result - result_opencv).max()}"
```

### Comparing `albucore-0.0.6/tests/test_normalize.py` & `albucore-0.0.7/tests/test_normalize.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,18 +28,21 @@
 ])
 def test_normalize_lut(img, denominator, mean, expected):
     num_channels = get_num_channels(img)
 
     converted_denominator = convert_value(denominator, num_channels)
     converted_mean = convert_value(mean, num_channels)
 
-    result = normalize_lut(img, converted_mean, converted_denominator)
+    result = normalize_lut(img, converted_mean, denominator)
+    result_lut = normalize_lut(img, converted_mean, converted_denominator)
     result_np = normalize_numpy(img, mean, denominator)
     result_cv2 = normalize_opencv(img, mean, denominator)
+
     np.array_equal(result, expected)
+    np.array_equal(result_lut, expected)
     np.array_equal(result_np, expected)
     np.array_equal(result_cv2, expected)
 
 
 @pytest.mark.parametrize(
     ["image", "mean", "std"],
     [
@@ -74,14 +77,14 @@
 
 
 @pytest.mark.parametrize("dtype", [
     np.uint8,
     np.float32,
 ])
 @pytest.mark.parametrize("shape", [(99, 101, 3), (99, 101, 1), (99, 101)])
-def test_normalize_float(dtype, shape) -> None:
+def test_normalize(dtype, shape) -> None:
     img = np.ones(shape, dtype=dtype) * 0.4
     mean = np.array(50, dtype=np.float32)
     denominator = np.array(1 / 3, dtype=np.float32)
     normalized = normalize(img, mean=mean, denominator=denominator)
     expected = (np.ones(img.shape, dtype=np.float32) * 0.4 - 50) / 3
     assert_array_almost_equal_nulp(normalized, expected)
```

### Comparing `albucore-0.0.6/tests/test_utils.py` & `albucore-0.0.7/tests/test_utils.py`

 * *Files identical despite different names*

