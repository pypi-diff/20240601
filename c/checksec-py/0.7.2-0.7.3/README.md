# Comparing `tmp/checksec_py-0.7.2.tar.gz` & `tmp/checksec_py-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checksec_py-0.7.2.tar", max compression
+gzip compressed data, was "checksec_py-0.7.3.tar", max compression
```

## Comparing `checksec_py-0.7.2.tar` & `checksec_py-0.7.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35149 2024-05-20 02:56:59.107905 checksec_py-0.7.2/LICENSE
--rw-r--r--   0        0        0     8657 2024-05-20 02:56:59.107905 checksec_py-0.7.2/README.md
--rw-r--r--   0        0        0        0 2024-05-20 02:56:59.107905 checksec_py-0.7.2/checksec/__init__.py
--rw-r--r--   0        0        0     5901 2024-05-20 02:56:59.107905 checksec_py-0.7.2/checksec/__main__.py
--rw-r--r--   0        0        0      616 2024-05-20 02:56:59.107905 checksec_py-0.7.2/checksec/binary.py
--rw-r--r--   0        0        0     7384 2024-05-20 02:56:59.107905 checksec_py-0.7.2/checksec/elf.py
--rw-r--r--   0        0        0      218 2024-05-20 02:56:59.107905 checksec_py-0.7.2/checksec/errors.py
--rw-r--r--   0        0        0    13391 2024-05-20 02:56:59.107905 checksec_py-0.7.2/checksec/output.py
--rw-r--r--   0        0        0     4397 2024-05-20 02:56:59.107905 checksec_py-0.7.2/checksec/pe.py
--rw-r--r--   0        0        0     4852 2024-05-20 02:56:59.107905 checksec_py-0.7.2/checksec/utils.py
--rw-r--r--   0        0        0     1385 2024-05-20 02:56:59.107905 checksec_py-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     9479 1970-01-01 00:00:00.000000 checksec_py-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-31 22:18:27.741862 checksec_py-0.7.3/LICENSE
+-rw-r--r--   0        0        0     8657 2024-05-31 22:18:27.741862 checksec_py-0.7.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-31 22:18:27.741862 checksec_py-0.7.3/checksec/__init__.py
+-rw-r--r--   0        0        0     5901 2024-05-31 22:18:27.741862 checksec_py-0.7.3/checksec/__main__.py
+-rw-r--r--   0        0        0      616 2024-05-31 22:18:27.741862 checksec_py-0.7.3/checksec/binary.py
+-rw-r--r--   0        0        0     7384 2024-05-31 22:18:27.741862 checksec_py-0.7.3/checksec/elf.py
+-rw-r--r--   0        0        0      218 2024-05-31 22:18:27.741862 checksec_py-0.7.3/checksec/errors.py
+-rw-r--r--   0        0        0    13422 2024-05-31 22:18:27.745862 checksec_py-0.7.3/checksec/output.py
+-rw-r--r--   0        0        0     4585 2024-05-31 22:18:27.745862 checksec_py-0.7.3/checksec/pe.py
+-rw-r--r--   0        0        0     4852 2024-05-31 22:18:27.745862 checksec_py-0.7.3/checksec/utils.py
+-rw-r--r--   0        0        0     1385 2024-05-31 22:18:27.745862 checksec_py-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     9486 1970-01-01 00:00:00.000000 checksec_py-0.7.3/PKG-INFO
```

### Comparing `checksec_py-0.7.2/LICENSE` & `checksec_py-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `checksec_py-0.7.2/README.md` & `checksec_py-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `checksec_py-0.7.2/checksec/__main__.py` & `checksec_py-0.7.3/checksec/__main__.py`

 * *Files identical despite different names*

### Comparing `checksec_py-0.7.2/checksec/binary.py` & `checksec_py-0.7.3/checksec/binary.py`

 * *Files identical despite different names*

### Comparing `checksec_py-0.7.2/checksec/elf.py` & `checksec_py-0.7.3/checksec/elf.py`

 * *Files identical despite different names*

### Comparing `checksec_py-0.7.2/checksec/output.py` & `checksec_py-0.7.3/checksec/output.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import json
 import logging
 from abc import ABC, abstractmethod
 from pathlib import Path
 from typing import List, Union
 
-from lief.PE import MACHINE_TYPES
+from lief.PE import Header
 from rich.console import Console
 from rich.progress import BarColumn, Progress, TextColumn
 from rich.table import Table
 
 from checksec.elf import ELFChecksecData, PIEType, RelroType
 from checksec.pe import PEChecksecData
 
+MACHINE_TYPES = Header.MACHINE_TYPES
+
 
 class AbstractChecksecOutput(ABC):
     def __init__(self, libc_detected: bool = False):
         self._libc_detected = libc_detected
         self.total = None
 
     def __enter__(self):
```

### Comparing `checksec_py-0.7.2/checksec/pe.py` & `checksec_py-0.7.3/checksec/pe.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from collections import namedtuple
 from pathlib import Path
 
 import lief
-from lief.PE import DLL_CHARACTERISTICS, HEADER_CHARACTERISTICS, MACHINE_TYPES, Signature
+from lief.PE import Header, OptionalHeader, Signature
 
 from .binary import BinarySecurity
 
+DLL_CHARACTERISTICS = OptionalHeader.DLL_CHARACTERISTICS
+HEADER_CHARACTERISTICS = Header.CHARACTERISTICS
+MACHINE_TYPES = Header.MACHINE_TYPES
+
 PEChecksecData = namedtuple(
     "PEChecksecData",
     [
         "machine",
         "nx",
         "canary",
         "aslr",
@@ -109,16 +113,18 @@
         """Whether manifest isolation is enabled"""
         # MSDN doc: https://docs.microsoft.com/en-us/cpp/build/reference/allowisolation-manifest-lookup?view=vs-2019
         # November 2016
         return not self.bin.optional_header.has(DLL_CHARACTERISTICS.NO_ISOLATION)
 
     @property
     def checksec_state(self) -> PEChecksecData:
+        machine: MACHINE_TYPES = self.bin.header.machine
+        machine_int = machine.value
         return PEChecksecData(
-            machine=self.bin.header.machine,
+            machine=machine_int,
             nx=self.has_nx,
             canary=self.has_canary,
             aslr=self.is_aslr,
             dynamic_base=self.has_dynamic_base,
             high_entropy_va=self.has_high_entropy_va,
             seh=self.has_seh,
             safe_seh=self.has_safe_seh,
```

### Comparing `checksec_py-0.7.2/checksec/utils.py` & `checksec_py-0.7.3/checksec/utils.py`

 * *Files identical despite different names*

### Comparing `checksec_py-0.7.2/pyproject.toml` & `checksec_py-0.7.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "checksec-py"
-version = "0.7.2"
+version = "0.7.3"
 description = "Checksec tool implemented in Python"
 authors = ["Mathieu Tarral <mathieu.tarral@protonmail.com>"]
 readme = "README.md"
-packages = [{include = "checksec"}]
+packages = [{ include = "checksec" }]
 license = "GPL-3.0-only"
 repository = "https://github.com/Wenzel/checksec.py"
 keywords = ["checksec", "security", "ELF", "PE", "binary"]
 
 [tool.poetry.scripts]
 checksec = 'checksec.__main__:entrypoint'
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.13"
-lief = "0.13.0"
+lief = "0.14.1"
 docopt = "0.6.2"
-rich = "13.3.5"
-pylddwrap = "1.0.1"
+rich = "^13.4"
+pylddwrap = "^1.0"
 
 [tool.poetry.dev-dependencies]
 flake8 = "5.0.4"
 flake8-bugbear = "20.1.4"
 isort = "5.10.1"
 black = "24.3.0"
 mypy = "1.2.0"
```

### Comparing `checksec_py-0.7.2/PKG-INFO` & `checksec_py-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: checksec-py
-Version: 0.7.2
+Version: 0.7.3
 Summary: Checksec tool implemented in Python
 Home-page: https://github.com/Wenzel/checksec.py
 License: GPL-3.0-only
 Keywords: checksec,security,ELF,PE,binary
 Author: Mathieu Tarral
 Author-email: mathieu.tarral@protonmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: docopt (==0.6.2)
-Requires-Dist: lief (==0.13.0)
-Requires-Dist: pylddwrap (==1.0.1)
-Requires-Dist: rich (==13.3.5)
+Requires-Dist: lief (==0.14.1)
+Requires-Dist: pylddwrap (>=1.0,<2.0)
+Requires-Dist: rich (>=13.4,<14.0)
 Project-URL: Repository, https://github.com/Wenzel/checksec.py
 Description-Content-Type: text/markdown
 
 <h1 align="center">
   <br>checksec.py</br>
 </h1>
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: checksec-py Version: 0.7.2 Summary: Checksec tool
+Metadata-Version: 2.1 Name: checksec-py Version: 0.7.3 Summary: Checksec tool
 implemented in Python Home-page: https://github.com/Wenzel/checksec.py License:
 GPL-3.0-only Keywords: checksec,security,ELF,PE,binary Author: Mathieu Tarral
 Author-email: mathieu.tarral@protonmail.com Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Dist: docopt
-(==0.6.2) Requires-Dist: lief (==0.13.0) Requires-Dist: pylddwrap (==1.0.1)
-Requires-Dist: rich (==13.3.5) Project-URL: Repository, https://github.com/
+(==0.6.2) Requires-Dist: lief (==0.14.1) Requires-Dist: pylddwrap (>=1.0,<2.0)
+Requires-Dist: rich (>=13.4,<14.0) Project-URL: Repository, https://github.com/
 Wenzel/checksec.py Description-Content-Type: text/markdown
                                     ************
                               cchheecckksseecc..ppyy ************
          ******** CChheecckksseecc ttooooll iinn PPyytthhoonn,, RRiicchh oouuttppuutt,, bbaasseedd oonn LLIIEEFF ********
                                      _DD_ee_mm_oo
 _[_C_I_ _b_a_d_g_e_]_[_P_y_P_I_ _p_a_c_k_a_g_e_ _b_a_d_g_e_]_[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_ _b_a_d_g_e_]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_s_._g_i_t_t_e_r_._i_m_/
                           _c_h_e_c_k_s_e_c_-_p_y_/_c_o_m_m_u_n_i_t_y_._s_v_g_]
```

