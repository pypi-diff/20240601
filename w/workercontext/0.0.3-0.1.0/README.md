# Comparing `tmp/workercontext-0.0.3.tar.gz` & `tmp/workercontext-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "workercontext-0.0.3.tar", last modified: Wed Apr 26 09:52:39 2023, max compression
+gzip compressed data, was "workercontext-0.1.0.tar", last modified: Sat Jun  1 02:04:22 2024, max compression
```

## Comparing `workercontext-0.0.3.tar` & `workercontext-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 09:52:39.238947 workercontext-0.0.3/
--rw-rw-rw-   0        0        0     1088 2023-04-26 08:49:47.000000 workercontext-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     6043 2023-04-26 09:52:39.235945 workercontext-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     4179 2023-04-26 09:51:06.000000 workercontext-0.0.3/README.md
--rw-rw-rw-   0        0        0      738 2023-04-26 09:50:36.000000 workercontext-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-26 09:52:39.238947 workercontext-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-26 09:52:39.181948 workercontext-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-26 09:52:39.203945 workercontext-0.0.3/src/workercontext/
--rw-rw-rw-   0        0        0       37 2023-04-26 09:18:25.000000 workercontext-0.0.3/src/workercontext/__init__.py
--rw-rw-rw-   0        0        0     4254 2023-04-26 09:07:24.000000 workercontext-0.0.3/src/workercontext/multiworker.py
--rw-rw-rw-   0        0        0     4069 2023-04-26 08:33:40.000000 workercontext-0.0.3/src/workercontext/reductions.py
-drwxrwxrwx   0        0        0        0 2023-04-26 09:52:39.216946 workercontext-0.0.3/src/workercontext.egg-info/
--rw-rw-rw-   0        0        0     6043 2023-04-26 09:52:39.000000 workercontext-0.0.3/src/workercontext.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      367 2023-04-26 09:52:39.000000 workercontext-0.0.3/src/workercontext.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 09:52:39.000000 workercontext-0.0.3/src/workercontext.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-26 09:52:39.000000 workercontext-0.0.3/src/workercontext.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-26 09:52:39.232948 workercontext-0.0.3/tests/
--rw-rw-rw-   0        0        0     2416 2023-04-26 09:07:46.000000 workercontext-0.0.3/tests/test_multiworker.py
--rw-rw-rw-   0        0        0     1291 2023-04-26 09:06:41.000000 workercontext-0.0.3/tests/test_performance.py
--rw-rw-rw-   0        0        0     2452 2023-04-26 09:06:54.000000 workercontext-0.0.3/tests/test_reduction.py
+drwxrwxrwx   0        0        0        0 2024-06-01 02:04:22.549301 workercontext-0.1.0/
+-rw-rw-rw-   0        0        0     1088 2023-04-26 08:49:47.000000 workercontext-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     7586 2024-06-01 02:04:22.547301 workercontext-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5722 2024-06-01 01:56:00.000000 workercontext-0.1.0/README.md
+-rw-rw-rw-   0        0        0      738 2024-06-01 01:56:00.000000 workercontext-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-01 02:04:22.549301 workercontext-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-01 02:04:22.522301 workercontext-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-06-01 02:04:22.530300 workercontext-0.1.0/src/workercontext/
+-rw-rw-rw-   0        0        0      137 2024-06-01 01:56:00.000000 workercontext-0.1.0/src/workercontext/__init__.py
+-rw-rw-rw-   0        0        0    11020 2024-06-01 01:56:00.000000 workercontext-0.1.0/src/workercontext/multiworker.py
+-rw-rw-rw-   0        0        0     4766 2024-06-01 01:56:00.000000 workercontext-0.1.0/src/workercontext/reductions.py
+drwxrwxrwx   0        0        0        0 2024-06-01 02:04:22.546300 workercontext-0.1.0/src/workercontext.egg-info/
+-rw-rw-rw-   0        0        0     7586 2024-06-01 02:04:22.000000 workercontext-0.1.0/src/workercontext.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2024-06-01 02:04:22.000000 workercontext-0.1.0/src/workercontext.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 02:04:22.000000 workercontext-0.1.0/src/workercontext.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-06-01 02:04:22.000000 workercontext-0.1.0/src/workercontext.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 02:04:22.545302 workercontext-0.1.0/tests/
+-rw-rw-rw-   0        0        0     1943 2024-06-01 01:56:00.000000 workercontext-0.1.0/tests/test_auto_parallelise.py
+-rw-rw-rw-   0        0        0     3248 2024-06-01 01:58:34.000000 workercontext-0.1.0/tests/test_multiworker.py
+-rw-rw-rw-   0        0        0     1546 2024-06-01 01:56:00.000000 workercontext-0.1.0/tests/test_multiworker_async.py
+-rw-rw-rw-   0        0        0     2261 2024-06-01 01:56:00.000000 workercontext-0.1.0/tests/test_parallelise.py
+-rw-rw-rw-   0        0        0     1291 2023-04-26 09:06:41.000000 workercontext-0.1.0/tests/test_performance.py
+-rw-rw-rw-   0        0        0     2450 2024-06-01 01:56:00.000000 workercontext-0.1.0/tests/test_reduction.py
```

### Comparing `workercontext-0.0.3/LICENSE` & `workercontext-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `workercontext-0.0.3/PKG-INFO` & `workercontext-0.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: workercontext
-Version: 0.0.3
+Version: 0.1.0
 Summary: A small package that provides a context to spin up multiple workers to execute a function
 Author-email: Owen Elliott <none@none.com>
 License: MIT License
         
         Copyright (c) 2023 Owen Elliott
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,14 +31,17 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Multi-Worker Context
 
+[![test](https://github.com/owenpendrighelliott/MultiWorker/actions/workflows/test.yml/badge.svg)](https://github.com/owenpendrighelliott/MultiWorker/actions/workflows/test.yml)
+
+
 This is a small project that create a context in python which can spin up multiple workers to do a task.
 
 The only requirement is that a the function you want to give multiple workers to has only one argument that you would like to batch on. It is up to you to ensure that creating independant batches for multiple workers makes sense with this argument.
 
 This makes refactoring code for multiprocessing a lot easier and should provide quick performance wins for time consuming functions with no interdependencies between elements.
 
 ## Setup
@@ -83,14 +86,34 @@
 with MultiWorker(my_func, n_processes=8, reduction=flatten_reduction) as f:
     res = f(arr)
 print(res)
 ```
 
 `res` will now a list of `int`.
 
+You can also parallelise functions without using the context manager:
+
+```python
+from workercontext import parallelise
+
+arr = list(range(100))
+
+res = parallelise(my_func, n_processes=8)(arr) # res is list of list of int
+```
+
+If you have type hints on your function then auto parallelise will guess the reduction to apply as well:
+
+```python
+from workercontext import auto_parallelise
+
+arr = list(range(100))
+
+res = auto_parallelise(my_func)(arr) # res is list of int
+```
+
 If you wanted to combine multiple reductions then you can use the reduction composition class
 
 ```python
 from workercontext import MultiWorker
 from workercontext.reductions import ReductionComposition, flatten_reduction, average_reduction
 
 reductions = ReductionComposition([flatten_reduction, average_reduction])
@@ -120,14 +143,47 @@
 arr2 = list(range(100))
 
 with MultiWorker(my_func, batched_arg='l2', n_processes=8, reduction=flatten_reduction) as f:
     res = f(arr1, arr2)
 print(res)
 ```
 
+## Async MultiWorker
+
+There is also an asynchroneous version of the MultiWorker context that does the processing async (non-blocking). You can either have it be async or have it converge when the context is exited.
+
+```python
+from workercontext import MultiWorkerAsync
+
+arr = list(range(100))
+
+res = [] # this is where the result will go
+
+with MultiWorkerAsync(my_func, n_processes=8, return_container=res) as f:
+    f(arr)
+    # do other things
+
+print(res) # res is gaurenteed to be populated AFTER context is exited
+```
+
+Or you can have no blocking by not specify a return container:
+
+```python
+from workercontext import MultiWorkerAsync, parallelise_async
+
+arr = list(range(100))
+
+# as a context 
+with MultiWorkerAsync(my_func, n_processes=8) as f:
+    f(arr)
+
+# or as a function
+parallelise_async(my_func, n_processes=8)(arr)
+```
+
 # Documentation
 
 ## MultiWorker
 ### parameters
 + `function` (`Callable`): The function to create the context for.
 + `n_processes` (`int`): The number of processes to spawn.
 + `batched_arg` (`str`, `optional`): The argument to batch on, if None the the first arg is used. Defaults to None.
```

### Comparing `workercontext-0.0.3/README.md` & `workercontext-0.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # Multi-Worker Context
 
+[![test](https://github.com/owenpendrighelliott/MultiWorker/actions/workflows/test.yml/badge.svg)](https://github.com/owenpendrighelliott/MultiWorker/actions/workflows/test.yml)
+
+
 This is a small project that create a context in python which can spin up multiple workers to do a task.
 
 The only requirement is that a the function you want to give multiple workers to has only one argument that you would like to batch on. It is up to you to ensure that creating independant batches for multiple workers makes sense with this argument.
 
 This makes refactoring code for multiprocessing a lot easier and should provide quick performance wins for time consuming functions with no interdependencies between elements.
 
 ## Setup
@@ -48,14 +51,34 @@
 with MultiWorker(my_func, n_processes=8, reduction=flatten_reduction) as f:
     res = f(arr)
 print(res)
 ```
 
 `res` will now a list of `int`.
 
+You can also parallelise functions without using the context manager:
+
+```python
+from workercontext import parallelise
+
+arr = list(range(100))
+
+res = parallelise(my_func, n_processes=8)(arr) # res is list of list of int
+```
+
+If you have type hints on your function then auto parallelise will guess the reduction to apply as well:
+
+```python
+from workercontext import auto_parallelise
+
+arr = list(range(100))
+
+res = auto_parallelise(my_func)(arr) # res is list of int
+```
+
 If you wanted to combine multiple reductions then you can use the reduction composition class
 
 ```python
 from workercontext import MultiWorker
 from workercontext.reductions import ReductionComposition, flatten_reduction, average_reduction
 
 reductions = ReductionComposition([flatten_reduction, average_reduction])
@@ -85,14 +108,47 @@
 arr2 = list(range(100))
 
 with MultiWorker(my_func, batched_arg='l2', n_processes=8, reduction=flatten_reduction) as f:
     res = f(arr1, arr2)
 print(res)
 ```
 
+## Async MultiWorker
+
+There is also an asynchroneous version of the MultiWorker context that does the processing async (non-blocking). You can either have it be async or have it converge when the context is exited.
+
+```python
+from workercontext import MultiWorkerAsync
+
+arr = list(range(100))
+
+res = [] # this is where the result will go
+
+with MultiWorkerAsync(my_func, n_processes=8, return_container=res) as f:
+    f(arr)
+    # do other things
+
+print(res) # res is gaurenteed to be populated AFTER context is exited
+```
+
+Or you can have no blocking by not specify a return container:
+
+```python
+from workercontext import MultiWorkerAsync, parallelise_async
+
+arr = list(range(100))
+
+# as a context 
+with MultiWorkerAsync(my_func, n_processes=8) as f:
+    f(arr)
+
+# or as a function
+parallelise_async(my_func, n_processes=8)(arr)
+```
+
 # Documentation
 
 ## MultiWorker
 ### parameters
 + `function` (`Callable`): The function to create the context for.
 + `n_processes` (`int`): The number of processes to spawn.
 + `batched_arg` (`str`, `optional`): The argument to batch on, if None the the first arg is used. Defaults to None.
```

### Comparing `workercontext-0.0.3/pyproject.toml` & `workercontext-0.1.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "workercontext"
-version = "0.0.3"
+version = "0.1.0"
 description = "A small package that provides a context to spin up multiple workers to execute a function"
 readme = "README.md"
 authors = [
   { name = "Owen Elliott", email = "none@none.com" },
 ]
 license = { file = "LICENSE" }
 classifiers = [
```

### Comparing `workercontext-0.0.3/src/workercontext/reductions.py` & `workercontext-0.1.0/src/workercontext/reductions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Dict, Union, Callable, Any
+from typing import List, Set, Dict, Union, Callable, Any
 
 
 class ReductionComposition:
     """Compose multiple reductions into a pipeline"""
 
     def __init__(self, reductions: List[Callable] = []):
         self._reductions = reductions
@@ -34,21 +34,53 @@
     """
     flattened = []
     for sublist in lst:
         flattened.extend(sublist)
     return flattened
 
 
+def set_union_reduction(lst: List[Set[Any]]) -> Set[Any]:
+    """
+    Returns the union of all the sets in the input list.
+
+    Args:
+        lst (List[Set[Any]]): A list of sets.
+
+    Returns:
+        Set[Any]: The union of all the sets in the input list.
+    """
+    union = set()
+    for s in lst:
+        union |= s
+    return union
+
+
+def dict_merge_reduction(lst: List[Dict[Any, Any]]) -> Dict[Any, Any]:
+    """
+    Returns the merge of all the dictionaries in the input list.
+
+    Args:
+        lst (List[Dict[Any, Any]]): A list of dictionaries.
+
+    Returns:
+        Dict[Any, Any]: The merge of all the dictionaries in the input list.
+    """
+    merged = {}
+    for d in lst:
+        merged.update(d)
+    return merged
+
+
 def sum_reduction(arr: List[float]) -> float:
     """
     Returns the sum of all the elements in the input array.
-    
+
     Args:
         arr (List[float]): A list of numbers.
-        
+
     Returns:
         float: The sum of all the elements in the input array.
     """
     result = 0
     for elem in arr:
         result += elem
     return result
@@ -65,78 +97,78 @@
         float: Average.
     """
     return sum(lst) / len(lst)
 
 
 def histogram_reduction(arr: List[Union[int, str]]) -> Dict[Union[int, str], int]:
     """Returns a dictionary containing the count of each unique element in the input array.
-    
+
     Args:
         arr (List[int]): A list of integers.
-        
+
     Returns:
         Dict[int, int]: A dictionary where keys are unique elements from the input array and values are their counts.
     """
     histogram = {}
     for elem in arr:
         if elem not in histogram:
             histogram[elem] = 1
         else:
             histogram[elem] += 1
     return histogram
 
 
 def product_reduction(arr: List[float]) -> float:
     """Returns the product of all the elements in the input array.
-    
+
     Args:
         arr (List[float]): A list of numbers.
-        
+
     Returns:
         float: The product of all the elements in the input array.
     """
     result = 1
     for elem in arr:
         result *= elem
     return result
 
 
 def string_concatenation_reduction(arr: List[str]) -> str:
     """Returns the concatenation of all the strings in the input array.
-    
+
     Args:
         arr (List[str]): A list of strings.
-        
+
     Returns:
         str: The concatenation of all the strings in the input array.
     """
     return "".join(arr)
 
 
 def bitwise_and_reduction(arr: List[int]) -> int:
     """Returns the bitwise AND of all the integers in the input array.
-    
+
     Args:
         arr (List[int]): A list of integers.
-        
+
     Returns:
         int: The bitwise AND of all the integers in the input array.
     """
     result = arr[0]
     for elem in arr[1:]:
         result &= elem
     return result
 
 
 def bitwise_or_reduction(arr: List[int]) -> int:
     """Returns the bitwise OR of all the integers in the input array.
-    
+
     Args:
         arr (List[int]): A list of integers.
-        
+
     Returns:
         int: The bitwise OR of all the integers in the input array.
     """
     result = arr[0]
     for elem in arr[1:]:
         result |= elem
     return result
```

### Comparing `workercontext-0.0.3/src/workercontext.egg-info/PKG-INFO` & `workercontext-0.1.0/src/workercontext.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: workercontext
-Version: 0.0.3
+Version: 0.1.0
 Summary: A small package that provides a context to spin up multiple workers to execute a function
 Author-email: Owen Elliott <none@none.com>
 License: MIT License
         
         Copyright (c) 2023 Owen Elliott
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,14 +31,17 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Multi-Worker Context
 
+[![test](https://github.com/owenpendrighelliott/MultiWorker/actions/workflows/test.yml/badge.svg)](https://github.com/owenpendrighelliott/MultiWorker/actions/workflows/test.yml)
+
+
 This is a small project that create a context in python which can spin up multiple workers to do a task.
 
 The only requirement is that a the function you want to give multiple workers to has only one argument that you would like to batch on. It is up to you to ensure that creating independant batches for multiple workers makes sense with this argument.
 
 This makes refactoring code for multiprocessing a lot easier and should provide quick performance wins for time consuming functions with no interdependencies between elements.
 
 ## Setup
@@ -83,14 +86,34 @@
 with MultiWorker(my_func, n_processes=8, reduction=flatten_reduction) as f:
     res = f(arr)
 print(res)
 ```
 
 `res` will now a list of `int`.
 
+You can also parallelise functions without using the context manager:
+
+```python
+from workercontext import parallelise
+
+arr = list(range(100))
+
+res = parallelise(my_func, n_processes=8)(arr) # res is list of list of int
+```
+
+If you have type hints on your function then auto parallelise will guess the reduction to apply as well:
+
+```python
+from workercontext import auto_parallelise
+
+arr = list(range(100))
+
+res = auto_parallelise(my_func)(arr) # res is list of int
+```
+
 If you wanted to combine multiple reductions then you can use the reduction composition class
 
 ```python
 from workercontext import MultiWorker
 from workercontext.reductions import ReductionComposition, flatten_reduction, average_reduction
 
 reductions = ReductionComposition([flatten_reduction, average_reduction])
@@ -120,14 +143,47 @@
 arr2 = list(range(100))
 
 with MultiWorker(my_func, batched_arg='l2', n_processes=8, reduction=flatten_reduction) as f:
     res = f(arr1, arr2)
 print(res)
 ```
 
+## Async MultiWorker
+
+There is also an asynchroneous version of the MultiWorker context that does the processing async (non-blocking). You can either have it be async or have it converge when the context is exited.
+
+```python
+from workercontext import MultiWorkerAsync
+
+arr = list(range(100))
+
+res = [] # this is where the result will go
+
+with MultiWorkerAsync(my_func, n_processes=8, return_container=res) as f:
+    f(arr)
+    # do other things
+
+print(res) # res is gaurenteed to be populated AFTER context is exited
+```
+
+Or you can have no blocking by not specify a return container:
+
+```python
+from workercontext import MultiWorkerAsync, parallelise_async
+
+arr = list(range(100))
+
+# as a context 
+with MultiWorkerAsync(my_func, n_processes=8) as f:
+    f(arr)
+
+# or as a function
+parallelise_async(my_func, n_processes=8)(arr)
+```
+
 # Documentation
 
 ## MultiWorker
 ### parameters
 + `function` (`Callable`): The function to create the context for.
 + `n_processes` (`int`): The number of processes to spawn.
 + `batched_arg` (`str`, `optional`): The argument to batch on, if None the the first arg is used. Defaults to None.
```

### Comparing `workercontext-0.0.3/tests/test_multiworker.py` & `workercontext-0.1.0/tests/test_multiworker.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,55 +37,87 @@
     return l
 
 
 def func_no_list(a, b, c):
     return a + b + c
 
 
-def test_one_worker(short_list, long_list):
+def func_no_annotations(l, a, b):
+    for i in range(len(l)):
+        l[i] = l[i] + a + b
+    return l
+
+
+def func_annotations_list_last(a: int, b: int, l: List[int]):
+    for i in range(len(l)):
+        l[i] = l[i] + a + b
+    return l
+
+
+def test_one_worker(short_list):
     with MultiWorker(func_no_kwargs, 1) as f:
         res = f(short_list, 1, 1)
     assert res[0][0] == 3 and res[0][-1] == 10
     assert len(res[0]) == len(short_list)
 
 
+def test_more_workers_than_elements(short_list):
+    with MultiWorker(func_no_kwargs, 50) as f:
+        res = f(short_list, 1, 1)
+    assert len(res) == len(short_list)
+
+
 def test_workers(short_list, long_list):
     with MultiWorker(func_no_kwargs, 4) as f:
         res = f(short_list, 1, 1)
     assert res[0][0] == 3 and res[-1][-1] == 10
     assert sum(map(len, res)) == len(short_list)
 
     with MultiWorker(func_no_kwargs, 10) as f:
         res = f(long_list, 1, 1)
     assert res[0][0] == 2 and res[-1][-1] == 1_000_001
     assert sum(map(len, res)) == len(long_list)
 
 
-def test_with_kwargs(short_list, long_list):
+def test_no_annotations(short_list):
+    with MultiWorker(func_no_annotations, 4) as f:
+        res = f(short_list, 1, 1)
+    assert res[0][0] == 3 and res[-1][-1] == 10
+    assert sum(map(len, res)) == len(short_list)
+
+
+def test_annotations_list_last(short_list):
+    with MultiWorker(func_annotations_list_last, 4) as f:
+        res = f(1, 1, short_list)
+    assert res[0][0] == 3 and res[-1][-1] == 10
+    assert sum(map(len, res)) == len(short_list)
+
+
+def test_with_kwargs(short_list):
     with MultiWorker(func_kwargs, 4) as f:
         res = f(short_list, b=1, a=1)
     assert res[0][0] == 3 and res[-1][-1] == 10
     assert sum(map(len, res)) == len(short_list)
 
 
-def test_only_kwargs(short_list, long_list):
+def test_only_kwargs(short_list):
     with MultiWorker(func_kwargs, 4) as f:
         res = f(l=short_list, b=1, a=1)
     assert res[0][0] == 3 and res[-1][-1] == 10
     assert sum(map(len, res)) == len(short_list)
 
 
-def test_second_arg_list(short_list, long_list):
+def test_second_arg_list(short_list):
     with MultiWorker(func_second_arg_list, 4, batched_arg="l") as f:
         res = f(l=short_list, b=1, a=1)
     assert res[0][0] == 3 and res[-1][-1] == 10
     assert sum(map(len, res)) == len(short_list)
 
 
-def test_invalid_param_error(short_list, long_list):
+def test_invalid_param_error():
     failed = False
     try:
         with MultiWorker(func_no_list, 4) as f:
             res = f(2, 2, 2)
     except ValueError:
         failed = True
```

### Comparing `workercontext-0.0.3/tests/test_performance.py` & `workercontext-0.1.0/tests/test_performance.py`

 * *Files identical despite different names*

### Comparing `workercontext-0.0.3/tests/test_reduction.py` & `workercontext-0.1.0/tests/test_reduction.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,11 +89,10 @@
 
     with MultiWorker(list_return, 4, reduction=reductions) as f:
         res = f(short_list)
     assert res == 10321920
 
 
 def test_string_concat(short_str_list):
-
     with MultiWorker(concat, 4, reduction=string_concatenation_reduction) as f:
         res = f(short_str_list)
     assert res == "".join(short_str_list)
```

