# Comparing `tmp/protloc_mex_x-0.0.8.tar.gz` & `tmp/protloc_mex_x-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protloc_mex_x-0.0.8.tar", max compression
+gzip compressed data, was "protloc_mex_x-0.0.9.tar", max compression
```

## Comparing `protloc_mex_x-0.0.8.tar` & `protloc_mex_x-0.0.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1091 2023-04-25 08:38:36.000000 protloc_mex_x-0.0.8/LICENSE.txt
--rw-r--r--   0        0        0        2 2023-05-09 03:41:02.000000 protloc_mex_x-0.0.8/protloc_mex_X/__init__.py
--rw-r--r--   0        0        0    39068 2023-06-01 11:45:18.000000 protloc_mex_x-0.0.8/protloc_mex_X/ESM2_fr.py
--rw-r--r--   0        0        0     2999 2023-05-08 12:33:04.000000 protloc_mex_x-0.0.8/protloc_mex_X/examples/test1.txt
--rw-r--r--   0        0        0     2749 2023-05-09 03:13:02.000000 protloc_mex_x-0.0.8/protloc_mex_X/feature_corrlation.py
--rw-r--r--   0        0        0      850 2023-09-09 09:28:39.812563 protloc_mex_x-0.0.8/pyproject.toml
--rw-r--r--   0        0        0    10445 2023-09-09 09:27:52.201523 protloc_mex_x-0.0.8/README.md
--rw-r--r--   0        0        0    11127 1970-01-01 00:00:00.000000 protloc_mex_x-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-04-25 08:38:36.000000 protloc_mex_x-0.0.9/LICENSE.txt
+-rw-r--r--   0        0        0        2 2023-05-09 03:41:02.000000 protloc_mex_x-0.0.9/protloc_mex_X/__init__.py
+-rw-r--r--   0        0        0    39068 2023-06-01 11:45:18.000000 protloc_mex_x-0.0.9/protloc_mex_X/ESM2_fr.py
+-rw-r--r--   0        0        0     2999 2023-05-08 12:33:04.000000 protloc_mex_x-0.0.9/protloc_mex_X/examples/test1.txt
+-rw-r--r--   0        0        0     2749 2023-05-09 03:13:02.000000 protloc_mex_x-0.0.9/protloc_mex_X/feature_corrlation.py
+-rw-r--r--   0        0        0      850 2023-09-09 09:47:15.123822 protloc_mex_x-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0    10533 2023-09-09 09:48:33.429368 protloc_mex_x-0.0.9/README.md
+-rw-r--r--   0        0        0    11211 1970-01-01 00:00:00.000000 protloc_mex_x-0.0.9/PKG-INFO
```

### Comparing `protloc_mex_x-0.0.8/LICENSE.txt` & `protloc_mex_x-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `protloc_mex_x-0.0.8/protloc_mex_X/ESM2_fr.py` & `protloc_mex_x-0.0.9/protloc_mex_X/ESM2_fr.py`

 * *Files identical despite different names*

### Comparing `protloc_mex_x-0.0.8/protloc_mex_X/examples/test1.txt` & `protloc_mex_x-0.0.9/protloc_mex_X/examples/test1.txt`

 * *Files identical despite different names*

### Comparing `protloc_mex_x-0.0.8/protloc_mex_X/feature_corrlation.py` & `protloc_mex_x-0.0.9/protloc_mex_X/feature_corrlation.py`

 * *Files identical despite different names*

### Comparing `protloc_mex_x-0.0.8/pyproject.toml` & `protloc_mex_x-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "protloc_mex_X"
-version = "0.0.8"
+version = "0.0.9"
 description = "..."
 authors = ["Ze Yu Luo <1024226968@qq.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/yujuan-zhang/ProtLoc-mexl"
 repository = "https://github.com/yujuan-zhang/ProtLoc-mexl"
 documentation = "https://github.com/yujuan-zhang/ProtLoc-mexl/issues"
```

### Comparing `protloc_mex_x-0.0.8/README.md` & `protloc_mex_x-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -115,24 +115,28 @@
 import os
 import protloc_mex_X
 from protloc_mex_X.ESM2_fr import NetPhos_classic_txt_DataFrame
 import random
 import re
 
 example_data = os.path.join(protloc_mex_X.__path__[0], "examples", "test1.txt")
+#The example_data is generated data from protein sequences analyzed using Netpho.
+
 with open(example_data, "r") as f:
      data = f.read()
 # print(data)
 pattern = r".*YES"
 
 result_df = NetPhos_classic_txt_DataFrame(pattern, data)
 result_df.loc[:,'Entry']=result_df.loc[:,'Sequence']
 
 """
-To generate a corresponding sequence randomly, please note that this is just an example. In real scenarios, accurate gene sequences should be used because Netpho only provides 6-bp phosphorylation sites, which are not complete gene sequences.
+To generate a corresponding sequence randomly, please note that this is just an example. 
+In real scenarios, accurate gene sequences should be used because Netpho only provides 6-bp phosphorylation sites,
+which are not complete gene sequences.
 Additionally, you need to convert the 'position' column in result_df to an integer type.
 """
 
 # Function to generate random amino acid sequence with a minimum length
 def generate_random_sequence(min_length):
     amino_acids = 'ACDEFGHIKLMNPQRSTVWY'  # 20 standard amino acids
     return ''.join(random.choice(amino_acids) for _ in range(min_length))
```

### Comparing `protloc_mex_x-0.0.8/PKG-INFO` & `protloc_mex_x-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protloc_mex_X
-Version: 0.0.8
+Version: 0.0.9
 Summary: ...
 Home-page: https://github.com/yujuan-zhang/ProtLoc-mexl
 License: MIT
 Author: Ze Yu Luo
 Author-email: 1024226968@qq.com
 Requires-Python: >=3.9
 Classifier: Development Status :: 3 - Alpha
@@ -139,24 +139,28 @@
 import os
 import protloc_mex_X
 from protloc_mex_X.ESM2_fr import NetPhos_classic_txt_DataFrame
 import random
 import re
 
 example_data = os.path.join(protloc_mex_X.__path__[0], "examples", "test1.txt")
+#The example_data is generated data from protein sequences analyzed using Netpho.
+
 with open(example_data, "r") as f:
      data = f.read()
 # print(data)
 pattern = r".*YES"
 
 result_df = NetPhos_classic_txt_DataFrame(pattern, data)
 result_df.loc[:,'Entry']=result_df.loc[:,'Sequence']
 
 """
-To generate a corresponding sequence randomly, please note that this is just an example. In real scenarios, accurate gene sequences should be used because Netpho only provides 6-bp phosphorylation sites, which are not complete gene sequences.
+To generate a corresponding sequence randomly, please note that this is just an example. 
+In real scenarios, accurate gene sequences should be used because Netpho only provides 6-bp phosphorylation sites,
+which are not complete gene sequences.
 Additionally, you need to convert the 'position' column in result_df to an integer type.
 """
 
 # Function to generate random amino acid sequence with a minimum length
 def generate_random_sequence(min_length):
     amino_acids = 'ACDEFGHIKLMNPQRSTVWY'  # 20 standard amino acids
     return ''.join(random.choice(amino_acids) for _ in range(min_length))
```

