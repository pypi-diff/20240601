# Comparing `tmp/Geode_Viewables-2.2.3-cp39-cp39-manylinux2014_x86_64.whl.zip` & `tmp/Geode_Viewables-2.2.3rc1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 177463 bytes, number of entries: 11
--rw-r--r--  2.0 unx       97 b- defN 24-Jun-01 01:43 geode_viewables/__init__.py
--rw-r--r--  2.0 unx     1260 b- defN 24-Jun-01 01:43 geode_viewables/conversion.py
--rw-r--r--  2.0 unx     1228 b- defN 24-Jun-01 01:43 geode_viewables/qem_proxy.py
--rwxr-xr-x  2.0 unx   187808 b- defN 24-Jun-01 01:43 geode_viewables/lib64/geode_viewables_py_conversion.cpython-39-x86_64-linux-gnu.so
--rwxr-xr-x  2.0 unx   192408 b- defN 24-Jun-01 01:43 geode_viewables/lib64/geode_viewables_py_qem_proxy.cpython-39-x86_64-linux-gnu.so
--rwxr-xr-x  2.0 unx    39376 b- defN 24-Jun-01 01:43 geode_viewables/lib64/libGeode-Viewables_conversion.so
--rwxr-xr-x  2.0 unx    47760 b- defN 24-Jun-01 01:43 geode_viewables/lib64/libGeode-Viewables_qem_proxy.so
--rw-r--r--  2.0 unx     1888 b- defN 24-Jun-01 01:43 Geode_Viewables-2.2.3.dist-info/METADATA
--rw-r--r--  2.0 unx      103 b- defN 24-Jun-01 01:43 Geode_Viewables-2.2.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 24-Jun-01 01:43 Geode_Viewables-2.2.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1088 b- defN 24-Jun-01 01:43 Geode_Viewables-2.2.3.dist-info/RECORD
-11 files, 473032 bytes uncompressed, 175577 bytes compressed:  62.9%
+Zip file size: 158560 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat      202 b- defN 24-May-30 08:29 geode_viewables/__init__.py
+-rw-rw-rw-  2.0 fat     1284 b- defN 24-May-30 08:29 geode_viewables/conversion.py
+-rw-rw-rw-  2.0 fat     1251 b- defN 24-May-30 08:29 geode_viewables/qem_proxy.py
+-rw-rw-rw-  2.0 fat    32768 b- defN 24-May-30 08:29 geode_viewables/bin/Geode-Viewables_conversion.dll
+-rw-rw-rw-  2.0 fat    58880 b- defN 24-May-30 08:29 geode_viewables/bin/Geode-Viewables_qem_proxy.dll
+-rw-rw-rw-  2.0 fat   156672 b- defN 24-May-30 08:29 geode_viewables/bin/geode_viewables_py_conversion.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   126464 b- defN 24-May-30 08:29 geode_viewables/bin/geode_viewables_py_qem_proxy.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     1954 b- defN 24-May-30 08:29 Geode_Viewables-2.2.3rc1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 24-May-30 08:29 Geode_Viewables-2.2.3rc1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       16 b- defN 24-May-30 08:29 Geode_Viewables-2.2.3rc1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1065 b- defN 24-May-30 08:29 Geode_Viewables-2.2.3rc1.dist-info/RECORD
+11 files, 380656 bytes uncompressed, 156722 bytes compressed:  58.8%
```

## zipnote {}

```diff
@@ -3,32 +3,32 @@
 
 Filename: geode_viewables/conversion.py
 Comment: 
 
 Filename: geode_viewables/qem_proxy.py
 Comment: 
 
-Filename: geode_viewables/lib64/geode_viewables_py_conversion.cpython-39-x86_64-linux-gnu.so
+Filename: geode_viewables/bin/Geode-Viewables_conversion.dll
 Comment: 
 
-Filename: geode_viewables/lib64/geode_viewables_py_qem_proxy.cpython-39-x86_64-linux-gnu.so
+Filename: geode_viewables/bin/Geode-Viewables_qem_proxy.dll
 Comment: 
 
-Filename: geode_viewables/lib64/libGeode-Viewables_conversion.so
+Filename: geode_viewables/bin/geode_viewables_py_conversion.cp39-win_amd64.pyd
 Comment: 
 
-Filename: geode_viewables/lib64/libGeode-Viewables_qem_proxy.so
+Filename: geode_viewables/bin/geode_viewables_py_qem_proxy.cp39-win_amd64.pyd
 Comment: 
 
-Filename: Geode_Viewables-2.2.3.dist-info/METADATA
+Filename: Geode_Viewables-2.2.3rc1.dist-info/METADATA
 Comment: 
 
-Filename: Geode_Viewables-2.2.3.dist-info/WHEEL
+Filename: Geode_Viewables-2.2.3rc1.dist-info/WHEEL
 Comment: 
 
-Filename: Geode_Viewables-2.2.3.dist-info/top_level.txt
+Filename: Geode_Viewables-2.2.3rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: Geode_Viewables-2.2.3.dist-info/RECORD
+Filename: Geode_Viewables-2.2.3rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geode_viewables/__init__.py

```diff
@@ -1,4 +1,7 @@
-## Copyright (c) 2019 - 2024 Geode-solutions
-
-from .conversion import *
-from .qem_proxy import *
+## Copyright (c) 2019 - 2024 Geode-solutions
+
+import os, pathlib
+os.add_dll_directory(pathlib.Path(__file__).parent.resolve().joinpath('bin'))
+
+from .conversion import *
+from .qem_proxy import *
```

## geode_viewables/conversion.py

```diff
@@ -1,26 +1,26 @@
-# Copyright (c) 2019 - 2024 Geode-solutions
-#
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in
-# all copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-
-import opengeode
-import opengeode_io
-import opengeode_geosciences
-
-from .lib64.geode_viewables_py_conversion import *
-ViewablesConversionLibrary.initialize()
+# Copyright (c) 2019 - 2024 Geode-solutions
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in
+# all copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+import opengeode
+import opengeode_io
+import opengeode_geosciences
+
+from .bin.geode_viewables_py_conversion import *
+ViewablesConversionLibrary.initialize()
```

## geode_viewables/qem_proxy.py

```diff
@@ -1,25 +1,25 @@
-# Copyright (c) 2019 - 2024 Geode-solutions
-#
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in
-# all copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-
-import opengeode
-import geode_common
-
-from .lib64.geode_viewables_py_qem_proxy import *
-ViewablesQEMProxyLibrary.initialize()
+# Copyright (c) 2019 - 2024 Geode-solutions
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in
+# all copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+import opengeode
+import geode_common
+
+from .bin.geode_viewables_py_qem_proxy import *
+ViewablesQEMProxyLibrary.initialize()
```

## Comparing `Geode_Viewables-2.2.3.dist-info/METADATA` & `Geode_Viewables-2.2.3rc1.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,40 @@
-Metadata-Version: 2.1
-Name: Geode-Viewables
-Version: 2.2.3
-Summary: Geode module to objects visualization
-Home-page: https://github.com/Geode-solutions/Geode-Viewables
-Author: Geode-solutions
-Author-email: contact@geode-solutions.com
-License: Proprietary
-Description-Content-Type: text/markdown
-Requires-Dist: geode-common ==31.*,>=31.2.0
-Requires-Dist: opengeode-core ==14.*,>=14.21.3
-Requires-Dist: opengeode-geosciences ==7.*,>=7.7.0
-Requires-Dist: opengeode-io ==6.*,>=6.5.1
-
-<h1 align="center">Geode-Viewables<sup><i>by Geode-solutions</i></sup></h1>
-<h3 align="center">Utilities to help visualizing OpenGeode objects</h3>
-
-<p align="center">
-  <img src="https://github.com/Geode-solutions/Geode-Viewables_private/workflows/CI/badge.svg" alt="Build Status">
-  <img src="https://github.com/Geode-solutions/Geode-Viewables_private/workflows/CD/badge.svg" alt="Deploy Status">
-  <img src="https://img.shields.io/github/release/Geode-solutions/Geode-Viewables_private.svg" alt="Version">
-  <img src="https://img.shields.io/pypi/v/geode-simplex" alt="PyPI" >
-</p>
-
-<p align="center">
-  <img src="https://img.shields.io/static/v1?label=Windows&logo=windows&logoColor=white&message=support&color=success" alt="Windows support">
-  <img src="https://img.shields.io/static/v1?label=Ubuntu&logo=Ubuntu&logoColor=white&message=support&color=success" alt="Ubuntu support">
-  <img src="https://img.shields.io/static/v1?label=Red%20Hat&logo=Red-Hat&logoColor=white&message=support&color=success" alt="Red Hat support">
-</p>
-
-<p align="center">
-  <img src="https://img.shields.io/badge/C%2B%2B-11-blue.svg" alt="Language">
-  <img src="https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg" alt="Semantic-release">
-  <a href="https://geode-solutions.com/#slack">
-    <img src="https://opengeode-slack-invite.herokuapp.com/badge.svg" alt="Slack invite">
-  </a>
-</p>
+Metadata-Version: 2.1
+Name: Geode-Viewables
+Version: 2.2.3rc1
+Summary: Geode module to objects visualization
+Home-page: https://github.com/Geode-solutions/Geode-Viewables
+Author: Geode-solutions
+Author-email: contact@geode-solutions.com
+License: Proprietary
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+Requires-Dist: geode-common ==31.*,>=31.2.0rc1
+Requires-Dist: opengeode-core ==14.*,>=14.21.1
+Requires-Dist: opengeode-geosciences ==7.*,>=7.7.0
+Requires-Dist: opengeode-io ==6.*,>=6.5.1
+
+<h1 align="center">Geode-Viewables<sup><i>by Geode-solutions</i></sup></h1>
+<h3 align="center">Utilities to help visualizing OpenGeode objects</h3>
+
+<p align="center">
+  <img src="https://github.com/Geode-solutions/Geode-Viewables_private/workflows/CI/badge.svg" alt="Build Status">
+  <img src="https://github.com/Geode-solutions/Geode-Viewables_private/workflows/CD/badge.svg" alt="Deploy Status">
+  <img src="https://img.shields.io/github/release/Geode-solutions/Geode-Viewables_private.svg" alt="Version">
+  <img src="https://img.shields.io/pypi/v/geode-simplex" alt="PyPI" >
+</p>
+
+<p align="center">
+  <img src="https://img.shields.io/static/v1?label=Windows&logo=windows&logoColor=white&message=support&color=success" alt="Windows support">
+  <img src="https://img.shields.io/static/v1?label=Ubuntu&logo=Ubuntu&logoColor=white&message=support&color=success" alt="Ubuntu support">
+  <img src="https://img.shields.io/static/v1?label=Red%20Hat&logo=Red-Hat&logoColor=white&message=support&color=success" alt="Red Hat support">
+</p>
+
+<p align="center">
+  <img src="https://img.shields.io/badge/C%2B%2B-11-blue.svg" alt="Language">
+  <img src="https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg" alt="Semantic-release">
+  <a href="https://geode-solutions.com/#slack">
+    <img src="https://opengeode-slack-invite.herokuapp.com/badge.svg" alt="Slack invite">
+  </a>
+</p>
+
+
```

### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: Geode-Viewables Version: 2.2.3 Summary: Geode
+Metadata-Version: 2.1 Name: Geode-Viewables Version: 2.2.3rc1 Summary: Geode
 module to objects visualization Home-page: https://github.com/Geode-solutions/
 Geode-Viewables Author: Geode-solutions Author-email: contact@geode-
-solutions.com License: Proprietary Description-Content-Type: text/markdown
-Requires-Dist: geode-common ==31.*,>=31.2.0 Requires-Dist: opengeode-core
-==14.*,>=14.21.3 Requires-Dist: opengeode-geosciences ==7.*,>=7.7.0 Requires-
-Dist: opengeode-io ==6.*,>=6.5.1
+solutions.com License: Proprietary Platform: UNKNOWN Description-Content-Type:
+text/markdown Requires-Dist: geode-common ==31.*,>=31.2.0rc1 Requires-Dist:
+opengeode-core ==14.*,>=14.21.1 Requires-Dist: opengeode-geosciences
+==7.*,>=7.7.0 Requires-Dist: opengeode-io ==6.*,>=6.5.1
                 ************ GGeeooddee--VViieewwaabblleessbbyy GGeeooddee--ssoolluuttiioonnss ************
            ******** UUttiilliittiieess ttoo hheellpp vviissuuaalliizziinngg OOppeennGGeeooddee oobbjjeeccttss ********
                  [Build Status][Deploy Status][Version][PyPI]
               [Windows support][Ubuntu support][Red Hat support]
                   [Language][Semantic-release]_[_S_l_a_c_k_ _i_n_v_i_t_e_]
```

