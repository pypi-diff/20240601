# Comparing `tmp/i2cpy-0.1.0b3.tar.gz` & `tmp/i2cpy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i2cpy-0.1.0b3.tar", last modified: Fri May 17 15:21:40 2024, max compression
+gzip compressed data, was "i2cpy-0.1.1.tar", last modified: Sat Jun  1 04:36:31 2024, max compression
```

## Comparing `i2cpy-0.1.0b3.tar` & `i2cpy-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 15:21:40.317047 i2cpy-0.1.0b3/
--rw-rw-rw-   0        0        0     1073 2024-05-05 19:00:07.000000 i2cpy-0.1.0b3/LICENSE
--rw-rw-rw-   0        0        0     8748 2024-05-17 15:21:40.315097 i2cpy-0.1.0b3/PKG-INFO
--rw-rw-rw-   0        0        0     6887 2024-05-17 15:19:17.000000 i2cpy-0.1.0b3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 15:21:40.256155 i2cpy-0.1.0b3/i2cpy/
--rw-rw-rw-   0        0        0     6642 2024-05-17 15:18:17.000000 i2cpy-0.1.0b3/i2cpy/__init__.py
--rw-rw-rw-   0        0        0       25 2024-05-17 15:21:16.000000 i2cpy-0.1.0b3/i2cpy/_version.py
-drwxrwxrwx   0        0        0        0 2024-05-17 15:21:40.284153 i2cpy-0.1.0b3/i2cpy/driver/
--rw-rw-rw-   0        0        0     3734 2024-05-13 11:28:11.000000 i2cpy-0.1.0b3/i2cpy/driver/abc.py
-drwxrwxrwx   0        0        0        0 2024-05-17 15:21:40.299374 i2cpy-0.1.0b3/i2cpy/driver/ch341/
--rw-rw-rw-   0        0        0     6347 2024-05-17 15:18:17.000000 i2cpy-0.1.0b3/i2cpy/driver/ch341/__init__.py
--rw-rw-rw-   0        0        0      278 2024-05-05 19:11:06.000000 i2cpy-0.1.0b3/i2cpy/driver/ch341/constants.py
--rw-rw-rw-   0        0        0     1282 2024-05-17 15:10:31.000000 i2cpy-0.1.0b3/i2cpy/driver/ch341/dll.py
--rw-rw-rw-   0        0        0      807 2024-05-17 15:18:17.000000 i2cpy-0.1.0b3/i2cpy/errors.py
-drwxrwxrwx   0        0        0        0 2024-05-17 15:21:40.313135 i2cpy-0.1.0b3/i2cpy.egg-info/
--rw-rw-rw-   0        0        0     8748 2024-05-17 15:21:40.000000 i2cpy-0.1.0b3/i2cpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      375 2024-05-17 15:21:40.000000 i2cpy-0.1.0b3/i2cpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 15:21:40.000000 i2cpy-0.1.0b3/i2cpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-05-17 15:21:40.000000 i2cpy-0.1.0b3/i2cpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-17 15:21:40.000000 i2cpy-0.1.0b3/i2cpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      816 2024-05-13 10:18:51.000000 i2cpy-0.1.0b3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-17 15:21:40.318026 i2cpy-0.1.0b3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-17 15:21:40.306255 i2cpy-0.1.0b3/tests/
--rw-rw-rw-   0        0        0      802 2024-05-12 14:58:02.000000 i2cpy-0.1.0b3/tests/test_i2c.py
--rw-rw-rw-   0        0        0      792 2024-05-13 10:18:51.000000 i2cpy-0.1.0b3/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-06-01 04:36:31.295797 i2cpy-0.1.1/
+-rw-rw-rw-   0        0        0     1073 2024-05-05 19:00:07.000000 i2cpy-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     9099 2024-06-01 04:36:31.293794 i2cpy-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6952 2024-05-21 18:24:21.000000 i2cpy-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 04:36:31.256280 i2cpy-0.1.1/i2cpy/
+-rw-rw-rw-   0        0        0     6709 2024-05-21 18:23:13.000000 i2cpy-0.1.1/i2cpy/__init__.py
+-rw-rw-rw-   0        0        0       23 2024-06-01 04:33:59.000000 i2cpy-0.1.1/i2cpy/_version.py
+drwxrwxrwx   0        0        0        0 2024-06-01 04:36:31.274795 i2cpy-0.1.1/i2cpy/driver/
+-rw-rw-rw-   0        0        0     3734 2024-05-13 11:28:11.000000 i2cpy-0.1.1/i2cpy/driver/abc.py
+drwxrwxrwx   0        0        0        0 2024-06-01 04:36:31.284798 i2cpy-0.1.1/i2cpy/driver/ch341/
+-rw-rw-rw-   0        0        0     6347 2024-05-17 15:18:17.000000 i2cpy-0.1.1/i2cpy/driver/ch341/__init__.py
+-rw-rw-rw-   0        0        0      278 2024-05-05 19:11:06.000000 i2cpy-0.1.1/i2cpy/driver/ch341/constants.py
+-rw-rw-rw-   0        0        0     1282 2024-05-17 15:10:31.000000 i2cpy-0.1.1/i2cpy/driver/ch341/dll.py
+-rw-rw-rw-   0        0        0      807 2024-05-17 15:18:17.000000 i2cpy-0.1.1/i2cpy/errors.py
+drwxrwxrwx   0        0        0        0 2024-06-01 04:36:31.291794 i2cpy-0.1.1/i2cpy.egg-info/
+-rw-rw-rw-   0        0        0     9099 2024-06-01 04:36:31.000000 i2cpy-0.1.1/i2cpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      375 2024-06-01 04:36:31.000000 i2cpy-0.1.1/i2cpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 04:36:31.000000 i2cpy-0.1.1/i2cpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-06-01 04:36:31.000000 i2cpy-0.1.1/i2cpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-06-01 04:36:31.000000 i2cpy-0.1.1/i2cpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1062 2024-06-01 04:32:20.000000 i2cpy-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-01 04:36:31.295797 i2cpy-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-01 04:36:31.288795 i2cpy-0.1.1/tests/
+-rw-rw-rw-   0        0        0      802 2024-05-12 14:58:02.000000 i2cpy-0.1.1/tests/test_i2c.py
+-rw-rw-rw-   0        0        0      792 2024-05-13 10:18:51.000000 i2cpy-0.1.1/tests/test_utils.py
```

### Comparing `i2cpy-0.1.0b3/LICENSE` & `i2cpy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `i2cpy-0.1.0b3/PKG-INFO` & `i2cpy-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i2cpy
-Version: 0.1.0b3
+Version: 0.1.1
 Summary: Python I2C library supporting multiple driver implementations
 Author-email: Zhenyi Zhou <iynehz@163.com>
 License: Copyright (c) 2024 Zhenyi Zhou
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
@@ -23,16 +23,22 @@
         LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
         OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
         WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 Project-URL: Homepage, https://github.com/iynehz/i2cpy
 Project-URL: Documentation, https://i2cpy.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/iynehz/i2cpy
 Keywords: i2c,ch341,ch341a
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Software Development
+Classifier: Topic :: Scientific/Engineering
+Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: typing_extensions>=4.6.0; python_version < "3.12"
 
 # Python I2C library supporting multiple driver implementations
 
@@ -49,16 +55,20 @@
 I2C is a two-wire protocol for communicating between devices. At the
 physical level it consists of 2 wires: SCL and SDA, the clock and data lines
 respectively.
 
 I2C objects are created attached to a specific bus. They can be initialized
 when created, or initialized later on.
 
-This library is designed to support different I2C driver implementations.
-It’s interface is similar to MicroPython’s `machine.I2C` as well as CircuitPython’s
+This library is designed to support different I2C driver implementations. At
+present below drivers are supported:
+
+* CH341 (CH341A, etc)
+
+The interface is similar to MicroPython’s `machine.I2C` as well as CircuitPython’s
 `board.I2C` classes.
 
 Example usage:
 
 ```python
 from i2cpy import I2C
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: i2cpy Version: 0.1.0b3 Summary: Python I2C library
+Metadata-Version: 2.1 Name: i2cpy Version: 0.1.1 Summary: Python I2C library
 supporting multiple driver implementations Author-email: Zhenyi Zhou
 163.com> License: Copyright (c) 2024 Zhenyi Zhou Permission is hereby granted,
 free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without
 restriction, including without limitation the rights to use, copy, modify,
 merge, publish, distribute, sublicense, and/or sell copies of the Software, and
 to permit persons to whom the Software is furnished to do so, subject to the
@@ -13,32 +13,37 @@
 PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 Project-URL: Homepage, https://github.com/iynehz/i2cpy Project-URL:
 Documentation, https://i2cpy.readthedocs.io/en/latest/ Project-URL: Repository,
 https://github.com/iynehz/i2cpy Keywords: i2c,ch341,ch341a Classifier:
-Development Status :: 4 - Beta Classifier: Programming Language :: Python
-Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
-LICENSE Requires-Dist: typing_extensions>=4.6.0; python_version < "3.12" #
-Python I2C library supporting multiple driver implementations
+Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
+:: MIT License Classifier: Programming Language :: Python Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3 :: Only Classifier: Topic :: Software Development Classifier: Topic ::
+Scientific/Engineering Classifier: Typing :: Typed Requires-Python: >=3.7
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+typing_extensions>=4.6.0; python_version < "3.12" # Python I2C library
+supporting multiple driver implementations
 [python]_[_p_y_p_i_]_[_l_i_c_e_n_s_e_][docs][lint]
 ## Introduction I2C is a two-wire protocol for communicating between devices.
 At the physical level it consists of 2 wires: SCL and SDA, the clock and data
 lines respectively. I2C objects are created attached to a specific bus. They
 can be initialized when created, or initialized later on. This library is
-designed to support different I2C driver implementations. Itâs interface is
-similar to MicroPythonâs `machine.I2C` as well as CircuitPythonâs
-`board.I2C` classes. Example usage: ```python from i2cpy import I2C i2c = I2C()
-# create I2C peripheral i2c.writeto(42, b'123') # write 3 bytes to peripheral
-with 7-bit address 42 i2c.readfrom(42, 4) # read 4 bytes from peripheral with
-7-bit address 42 i2c.readfrom_mem(42, 8, 3) # read 3 bytes from memory of
-peripheral 42, # starting at memory address 8 in the peripheral i2c.writeto_mem
-(42, 2, b'\x10') # write 1 byte to memory of peripheral 42, # starting at
-memory address 2 in the peripheral ``` ## Class I2C ### Constructor ####
+designed to support different I2C driver implementations. At present below
+drivers are supported: * CH341 (CH341A, etc) The interface is similar to
+MicroPythonâs `machine.I2C` as well as CircuitPythonâs `board.I2C` classes.
+Example usage: ```python from i2cpy import I2C i2c = I2C() # create I2C
+peripheral i2c.writeto(42, b'123') # write 3 bytes to peripheral with 7-bit
+address 42 i2c.readfrom(42, 4) # read 4 bytes from peripheral with 7-bit
+address 42 i2c.readfrom_mem(42, 8, 3) # read 3 bytes from memory of peripheral
+42, # starting at memory address 8 in the peripheral i2c.writeto_mem(42, 2,
+b'\x10') # write 1 byte to memory of peripheral 42, # starting at memory
+address 2 in the peripheral ``` ## Class I2C ### Constructor ####
 I2C.\_\_init_\_(id=None, \*, driver=None, freq=400000, auto_init=True,
 \*\*kwargs) Constructor. * **Parameters:** * **id** (`Union`[`int`, `str`,
 `None`]) â Identifies a particular I2C peripheral. Allowed values depend on
 the particular driver implementation. * **freq** (`int`) â I2C bus baudrate,
 defaults to 400000 * **driver** (`Optional`[`str`]) â I2C driver name. It
 corresponds to the I2C driver sub module name shipped with this library. For
 example âfooâ means module âi2cpy.driver.fooâ. If not specified, it
```

### Comparing `i2cpy-0.1.0b3/README.md` & `i2cpy-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,20 @@
 I2C is a two-wire protocol for communicating between devices. At the
 physical level it consists of 2 wires: SCL and SDA, the clock and data lines
 respectively.
 
 I2C objects are created attached to a specific bus. They can be initialized
 when created, or initialized later on.
 
-This library is designed to support different I2C driver implementations.
-It’s interface is similar to MicroPython’s `machine.I2C` as well as CircuitPython’s
+This library is designed to support different I2C driver implementations. At
+present below drivers are supported:
+
+* CH341 (CH341A, etc)
+
+The interface is similar to MicroPython’s `machine.I2C` as well as CircuitPython’s
 `board.I2C` classes.
 
 Example usage:
 
 ```python
 from i2cpy import I2C
```

#### html2text {}

```diff
@@ -1,22 +1,23 @@
 # Python I2C library supporting multiple driver implementations
 [python]_[_p_y_p_i_]_[_l_i_c_e_n_s_e_][docs][lint]
 ## Introduction I2C is a two-wire protocol for communicating between devices.
 At the physical level it consists of 2 wires: SCL and SDA, the clock and data
 lines respectively. I2C objects are created attached to a specific bus. They
 can be initialized when created, or initialized later on. This library is
-designed to support different I2C driver implementations. Itâs interface is
-similar to MicroPythonâs `machine.I2C` as well as CircuitPythonâs
-`board.I2C` classes. Example usage: ```python from i2cpy import I2C i2c = I2C()
-# create I2C peripheral i2c.writeto(42, b'123') # write 3 bytes to peripheral
-with 7-bit address 42 i2c.readfrom(42, 4) # read 4 bytes from peripheral with
-7-bit address 42 i2c.readfrom_mem(42, 8, 3) # read 3 bytes from memory of
-peripheral 42, # starting at memory address 8 in the peripheral i2c.writeto_mem
-(42, 2, b'\x10') # write 1 byte to memory of peripheral 42, # starting at
-memory address 2 in the peripheral ``` ## Class I2C ### Constructor ####
+designed to support different I2C driver implementations. At present below
+drivers are supported: * CH341 (CH341A, etc) The interface is similar to
+MicroPythonâs `machine.I2C` as well as CircuitPythonâs `board.I2C` classes.
+Example usage: ```python from i2cpy import I2C i2c = I2C() # create I2C
+peripheral i2c.writeto(42, b'123') # write 3 bytes to peripheral with 7-bit
+address 42 i2c.readfrom(42, 4) # read 4 bytes from peripheral with 7-bit
+address 42 i2c.readfrom_mem(42, 8, 3) # read 3 bytes from memory of peripheral
+42, # starting at memory address 8 in the peripheral i2c.writeto_mem(42, 2,
+b'\x10') # write 1 byte to memory of peripheral 42, # starting at memory
+address 2 in the peripheral ``` ## Class I2C ### Constructor ####
 I2C.\_\_init_\_(id=None, \*, driver=None, freq=400000, auto_init=True,
 \*\*kwargs) Constructor. * **Parameters:** * **id** (`Union`[`int`, `str`,
 `None`]) â Identifies a particular I2C peripheral. Allowed values depend on
 the particular driver implementation. * **freq** (`int`) â I2C bus baudrate,
 defaults to 400000 * **driver** (`Optional`[`str`]) â I2C driver name. It
 corresponds to the I2C driver sub module name shipped with this library. For
 example âfooâ means module âi2cpy.driver.fooâ. If not specified, it
```

### Comparing `i2cpy-0.1.0b3/i2cpy/__init__.py` & `i2cpy-0.1.1/i2cpy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 """I2C is a two-wire protocol for communicating between devices. At the
 physical level it consists of 2 wires: SCL and SDA, the clock and data lines
 respectively.
 
 I2C objects are created attached to a specific bus. They can be initialized
 when created, or initialized later on.
 
-This library is designed to support different I2C driver implementations.
-It's interface is similar to MicroPython's ``machine.I2C`` as well as CircuitPython's
+This library is designed to support different I2C driver implementations. At
+present below drivers are supported:
+
+* CH341 (CH341A, etc)
+
+The interface is similar to MicroPython's ``machine.I2C`` as well as CircuitPython's
 ``board.I2C`` classes.
 
 Example usage:
 
 .. code-block:: python
 
     from i2cpy import I2C
```

### Comparing `i2cpy-0.1.0b3/i2cpy/driver/abc.py` & `i2cpy-0.1.1/i2cpy/driver/abc.py`

 * *Files identical despite different names*

### Comparing `i2cpy-0.1.0b3/i2cpy/driver/ch341/__init__.py` & `i2cpy-0.1.1/i2cpy/driver/ch341/__init__.py`

 * *Files identical despite different names*

### Comparing `i2cpy-0.1.0b3/i2cpy/driver/ch341/dll.py` & `i2cpy-0.1.1/i2cpy/driver/ch341/dll.py`

 * *Files identical despite different names*

### Comparing `i2cpy-0.1.0b3/i2cpy/errors.py` & `i2cpy-0.1.1/i2cpy/errors.py`

 * *Files identical despite different names*

### Comparing `i2cpy-0.1.0b3/i2cpy.egg-info/PKG-INFO` & `i2cpy-0.1.1/i2cpy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i2cpy
-Version: 0.1.0b3
+Version: 0.1.1
 Summary: Python I2C library supporting multiple driver implementations
 Author-email: Zhenyi Zhou <iynehz@163.com>
 License: Copyright (c) 2024 Zhenyi Zhou
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
@@ -23,16 +23,22 @@
         LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
         OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
         WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 Project-URL: Homepage, https://github.com/iynehz/i2cpy
 Project-URL: Documentation, https://i2cpy.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/iynehz/i2cpy
 Keywords: i2c,ch341,ch341a
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Software Development
+Classifier: Topic :: Scientific/Engineering
+Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: typing_extensions>=4.6.0; python_version < "3.12"
 
 # Python I2C library supporting multiple driver implementations
 
@@ -49,16 +55,20 @@
 I2C is a two-wire protocol for communicating between devices. At the
 physical level it consists of 2 wires: SCL and SDA, the clock and data lines
 respectively.
 
 I2C objects are created attached to a specific bus. They can be initialized
 when created, or initialized later on.
 
-This library is designed to support different I2C driver implementations.
-It’s interface is similar to MicroPython’s `machine.I2C` as well as CircuitPython’s
+This library is designed to support different I2C driver implementations. At
+present below drivers are supported:
+
+* CH341 (CH341A, etc)
+
+The interface is similar to MicroPython’s `machine.I2C` as well as CircuitPython’s
 `board.I2C` classes.
 
 Example usage:
 
 ```python
 from i2cpy import I2C
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: i2cpy Version: 0.1.0b3 Summary: Python I2C library
+Metadata-Version: 2.1 Name: i2cpy Version: 0.1.1 Summary: Python I2C library
 supporting multiple driver implementations Author-email: Zhenyi Zhou
 163.com> License: Copyright (c) 2024 Zhenyi Zhou Permission is hereby granted,
 free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without
 restriction, including without limitation the rights to use, copy, modify,
 merge, publish, distribute, sublicense, and/or sell copies of the Software, and
 to permit persons to whom the Software is furnished to do so, subject to the
@@ -13,32 +13,37 @@
 PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 Project-URL: Homepage, https://github.com/iynehz/i2cpy Project-URL:
 Documentation, https://i2cpy.readthedocs.io/en/latest/ Project-URL: Repository,
 https://github.com/iynehz/i2cpy Keywords: i2c,ch341,ch341a Classifier:
-Development Status :: 4 - Beta Classifier: Programming Language :: Python
-Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
-LICENSE Requires-Dist: typing_extensions>=4.6.0; python_version < "3.12" #
-Python I2C library supporting multiple driver implementations
+Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
+:: MIT License Classifier: Programming Language :: Python Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3 :: Only Classifier: Topic :: Software Development Classifier: Topic ::
+Scientific/Engineering Classifier: Typing :: Typed Requires-Python: >=3.7
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+typing_extensions>=4.6.0; python_version < "3.12" # Python I2C library
+supporting multiple driver implementations
 [python]_[_p_y_p_i_]_[_l_i_c_e_n_s_e_][docs][lint]
 ## Introduction I2C is a two-wire protocol for communicating between devices.
 At the physical level it consists of 2 wires: SCL and SDA, the clock and data
 lines respectively. I2C objects are created attached to a specific bus. They
 can be initialized when created, or initialized later on. This library is
-designed to support different I2C driver implementations. Itâs interface is
-similar to MicroPythonâs `machine.I2C` as well as CircuitPythonâs
-`board.I2C` classes. Example usage: ```python from i2cpy import I2C i2c = I2C()
-# create I2C peripheral i2c.writeto(42, b'123') # write 3 bytes to peripheral
-with 7-bit address 42 i2c.readfrom(42, 4) # read 4 bytes from peripheral with
-7-bit address 42 i2c.readfrom_mem(42, 8, 3) # read 3 bytes from memory of
-peripheral 42, # starting at memory address 8 in the peripheral i2c.writeto_mem
-(42, 2, b'\x10') # write 1 byte to memory of peripheral 42, # starting at
-memory address 2 in the peripheral ``` ## Class I2C ### Constructor ####
+designed to support different I2C driver implementations. At present below
+drivers are supported: * CH341 (CH341A, etc) The interface is similar to
+MicroPythonâs `machine.I2C` as well as CircuitPythonâs `board.I2C` classes.
+Example usage: ```python from i2cpy import I2C i2c = I2C() # create I2C
+peripheral i2c.writeto(42, b'123') # write 3 bytes to peripheral with 7-bit
+address 42 i2c.readfrom(42, 4) # read 4 bytes from peripheral with 7-bit
+address 42 i2c.readfrom_mem(42, 8, 3) # read 3 bytes from memory of peripheral
+42, # starting at memory address 8 in the peripheral i2c.writeto_mem(42, 2,
+b'\x10') # write 1 byte to memory of peripheral 42, # starting at memory
+address 2 in the peripheral ``` ## Class I2C ### Constructor ####
 I2C.\_\_init_\_(id=None, \*, driver=None, freq=400000, auto_init=True,
 \*\*kwargs) Constructor. * **Parameters:** * **id** (`Union`[`int`, `str`,
 `None`]) â Identifies a particular I2C peripheral. Allowed values depend on
 the particular driver implementation. * **freq** (`int`) â I2C bus baudrate,
 defaults to 400000 * **driver** (`Optional`[`str`]) â I2C driver name. It
 corresponds to the I2C driver sub module name shipped with this library. For
 example âfooâ means module âi2cpy.driver.fooâ. If not specified, it
```

### Comparing `i2cpy-0.1.0b3/tests/test_i2c.py` & `i2cpy-0.1.1/tests/test_i2c.py`

 * *Files identical despite different names*

### Comparing `i2cpy-0.1.0b3/tests/test_utils.py` & `i2cpy-0.1.1/tests/test_utils.py`

 * *Files identical despite different names*

