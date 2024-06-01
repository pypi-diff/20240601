# Comparing `tmp/chaos_stratus-1.0.1.tar.gz` & `tmp/chaos_stratus-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chaos_stratus-1.0.1.tar", last modified: Mon May 27 12:15:50 2024, max compression
+gzip compressed data, was "chaos_stratus-1.1.0.tar", last modified: Sat Jun  1 15:52:45 2024, max compression
```

## Comparing `chaos_stratus-1.0.1.tar` & `chaos_stratus-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 jbartle9  (1000) jbartle9  (1000)        0 2024-05-27 12:15:50.230155 chaos_stratus-1.0.1/
--rw-r--r--   0 jbartle9  (1000) jbartle9  (1000)     3450 2024-05-27 12:15:50.230155 chaos_stratus-1.0.1/PKG-INFO
--rw-rw-r--   0 jbartle9  (1000) jbartle9  (1000)     2981 2024-05-27 12:14:44.000000 chaos_stratus-1.0.1/README.md
--rw-rw-r--   0 jbartle9  (1000) jbartle9  (1000)      631 2024-05-27 12:15:14.000000 chaos_stratus-1.0.1/pyproject.toml
--rw-rw-r--   0 jbartle9  (1000) jbartle9  (1000)       38 2024-05-27 12:15:50.230155 chaos_stratus-1.0.1/setup.cfg
-drwxrwxr-x   0 jbartle9  (1000) jbartle9  (1000)        0 2024-05-27 12:15:50.230155 chaos_stratus-1.0.1/src/
-drwxrwxr-x   0 jbartle9  (1000) jbartle9  (1000)        0 2024-05-27 12:15:50.230155 chaos_stratus-1.0.1/src/chaos_stratus/
--rw-rw-r--   0 jbartle9  (1000) jbartle9  (1000)      234 2024-05-27 12:15:45.000000 chaos_stratus-1.0.1/src/chaos_stratus/__init__.py
--rw-rw-r--   0 jbartle9  (1000) jbartle9  (1000)      426 2024-05-27 07:43:44.000000 chaos_stratus-1.0.1/src/chaos_stratus/__main__.py
--rw-rw-r--   0 jbartle9  (1000) jbartle9  (1000)    11668 2024-05-27 09:03:17.000000 chaos_stratus-1.0.1/src/chaos_stratus/stratus.py
-drwxrwxr-x   0 jbartle9  (1000) jbartle9  (1000)        0 2024-05-27 12:15:50.230155 chaos_stratus-1.0.1/src/chaos_stratus.egg-info/
--rw-r--r--   0 jbartle9  (1000) jbartle9  (1000)     3450 2024-05-27 12:15:50.000000 chaos_stratus-1.0.1/src/chaos_stratus.egg-info/PKG-INFO
--rw-rw-r--   0 jbartle9  (1000) jbartle9  (1000)      277 2024-05-27 12:15:50.000000 chaos_stratus-1.0.1/src/chaos_stratus.egg-info/SOURCES.txt
--rw-rw-r--   0 jbartle9  (1000) jbartle9  (1000)        1 2024-05-27 12:15:50.000000 chaos_stratus-1.0.1/src/chaos_stratus.egg-info/dependency_links.txt
--rw-rw-r--   0 jbartle9  (1000) jbartle9  (1000)       14 2024-05-27 12:15:50.000000 chaos_stratus-1.0.1/src/chaos_stratus.egg-info/top_level.txt
+drwxrwxr-x   0 jbartle9  (1000) jbartle9  (1000)        0 2024-06-01 15:52:45.832331 chaos_stratus-1.1.0/
+-rw-r--r--   0 jbartle9  (1000) jbartle9  (1000)     3799 2024-06-01 15:52:45.832331 chaos_stratus-1.1.0/PKG-INFO
+-rw-rw-r--   0 jbartle9  (1000) jbartle9  (1000)     3355 2024-06-01 15:05:23.000000 chaos_stratus-1.1.0/README.md
+-rw-rw-r--   0 jbartle9  (1000) jbartle9  (1000)      606 2024-06-01 15:47:41.000000 chaos_stratus-1.1.0/pyproject.toml
+-rw-rw-r--   0 jbartle9  (1000) jbartle9  (1000)       38 2024-06-01 15:52:45.832331 chaos_stratus-1.1.0/setup.cfg
+drwxrwxr-x   0 jbartle9  (1000) jbartle9  (1000)        0 2024-06-01 15:52:45.832331 chaos_stratus-1.1.0/src/
+drwxrwxr-x   0 jbartle9  (1000) jbartle9  (1000)        0 2024-06-01 15:52:45.832331 chaos_stratus-1.1.0/src/chaos_stratus/
+-rw-rw-r--   0 jbartle9  (1000) jbartle9  (1000)      234 2024-05-27 12:15:45.000000 chaos_stratus-1.1.0/src/chaos_stratus/__init__.py
+-rw-rw-r--   0 jbartle9  (1000) jbartle9  (1000)      468 2024-06-01 15:45:38.000000 chaos_stratus-1.1.0/src/chaos_stratus/__main__.py
+-rw-rw-r--   0 jbartle9  (1000) jbartle9  (1000)    14544 2024-06-01 15:46:51.000000 chaos_stratus-1.1.0/src/chaos_stratus/stratus.py
+drwxrwxr-x   0 jbartle9  (1000) jbartle9  (1000)        0 2024-06-01 15:52:45.832331 chaos_stratus-1.1.0/src/chaos_stratus.egg-info/
+-rw-r--r--   0 jbartle9  (1000) jbartle9  (1000)     3799 2024-06-01 15:52:45.000000 chaos_stratus-1.1.0/src/chaos_stratus.egg-info/PKG-INFO
+-rw-rw-r--   0 jbartle9  (1000) jbartle9  (1000)      277 2024-06-01 15:52:45.000000 chaos_stratus-1.1.0/src/chaos_stratus.egg-info/SOURCES.txt
+-rw-rw-r--   0 jbartle9  (1000) jbartle9  (1000)        1 2024-06-01 15:52:45.000000 chaos_stratus-1.1.0/src/chaos_stratus.egg-info/dependency_links.txt
+-rw-rw-r--   0 jbartle9  (1000) jbartle9  (1000)       14 2024-06-01 15:52:45.000000 chaos_stratus-1.1.0/src/chaos_stratus.egg-info/top_level.txt
```

### Comparing `chaos_stratus-1.0.1/PKG-INFO` & `chaos_stratus-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 Metadata-Version: 2.1
 Name: chaos-stratus
-Version: 1.0.1
-Summary: Python tools used to interact with (appropriately compiled) Chaos Stratus effect libraries
+Version: 1.1.0
+Summary: Python tools used to interact with Chaos Stratus effect libraries
 Author-email: Martin Bartlett <martin.j.bartlett@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/bassmanitram/chaos-stratus-python
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.0
+Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 
 
 # chaos-stratus
 
 This package provides tools for interacting with (appropriately compiled) [Chaos Audio Stratus pedal](https://chaosaudio.com/) effects libraries. 
 
-By "appropriately compiled" we mean built with the Stratus build tools available with the most recent versions of [Faust](https://faust.grame.fr/), or with the [Faust IDE](https://faustide.grame.fr/).
+By "appropriately compiled" we mean built with the Stratus build tools available with the most recent versions of [Faust](https://faust.grame.fr/), 
+or with the [Faust IDE](https://faustide.grame.fr/).
+
+Effects that are _not_ built with the Faust tools (e.g. those built before those tools became available) are still at least _partially_ compatible
+with the library - they may not provide the documented class attributes, but they will provide the operational functions that allow you
+to interact with them.
+
+In _all_ cases, though, the effect must be built for the platform upon which this class is used - that means performing a "local" build with the
+Faust tools (or by some other means) or installing this package on the Stratus pedal itself.
 
-(Note that prior to the full Faust integration of the Stratus development tools, effects libraries were built in such a way as to NOT be fully compatible with these tools).
 # Installation
 
 You can install this package using a standard `pip` invocation
 
 
 ```
 python -m pip install chaos-stratus
```

### Comparing `chaos_stratus-1.0.1/README.md` & `chaos_stratus-1.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 
 # chaos-stratus
 
 This package provides tools for interacting with (appropriately compiled) [Chaos Audio Stratus pedal](https://chaosaudio.com/) effects libraries. 
 
-By "appropriately compiled" we mean built with the Stratus build tools available with the most recent versions of [Faust](https://faust.grame.fr/), or with the [Faust IDE](https://faustide.grame.fr/).
+By "appropriately compiled" we mean built with the Stratus build tools available with the most recent versions of [Faust](https://faust.grame.fr/), 
+or with the [Faust IDE](https://faustide.grame.fr/).
+
+Effects that are _not_ built with the Faust tools (e.g. those built before those tools became available) are still at least _partially_ compatible
+with the library - they may not provide the documented class attributes, but they will provide the operational functions that allow you
+to interact with them.
+
+In _all_ cases, though, the effect must be built for the platform upon which this class is used - that means performing a "local" build with the
+Faust tools (or by some other means) or installing this package on the Stratus pedal itself.
 
-(Note that prior to the full Faust integration of the Stratus development tools, effects libraries were built in such a way as to NOT be fully compatible with these tools).
 # Installation
 
 You can install this package using a standard `pip` invocation
 
 
 ```
 python -m pip install chaos-stratus
```

### Comparing `chaos_stratus-1.0.1/pyproject.toml` & `chaos_stratus-1.1.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 [build-system]
 requires      = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chaos-stratus"
-version = "1.0.1"
-description = 'Python tools used to interact with (appropriately compiled) Chaos Stratus effect libraries'
+version = "1.1.0"
+description = 'Python tools used to interact with Chaos Stratus effect libraries'
 readme = "README.md"
 authors = [{ name = "Martin Bartlett", email = "martin.j.bartlett@gmail.com" }]
 license = {text = "MIT License"}
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 dependencies = []
-requires-python = ">=3.0"
+requires-python = ">=3.5"
 
 [project.urls]
 Homepage = "https://github.com/bassmanitram/chaos-stratus-python"
```

### Comparing `chaos_stratus-1.0.1/src/chaos_stratus/stratus.py` & `chaos_stratus-1.1.0/src/chaos_stratus/stratus.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,75 @@
 from ctypes import *
 from sys import argv
+import subprocess
+import re
 
 InstanceHandle = c_void_p
 FloatPointer = POINTER(c_float)
 
 class EffectLib:
+    #
+    # For each namespace, try to find the specified function
+    # until one actually elicits the function
+    #
+    def _find_func(self, func_name, args):
+        for ns in self.nameSpaces:
+            symb = '_ZN{}{}{}{}{}'.format(len(ns),ns,len(func_name),func_name,args)
+            func = getattr(self.lib,symb, None)
+            if func is not None:
+                return func
+        return None
+    
+    #
+    # Basically we troll through the SO file and dig out all the
+    # _ZTI.... symbols - these are, effectively, the symbol namespaces
+    # we have to deal with. In FACT, because of the way we trim out two
+    # "well known" namespaces, there should only be a max of one other
+    # found.
+    #
+    def _find_namespaces(self, file):
+        namespaces = []
+        with open(file, "rb") as f:
+            TAG = [b'_',b'Z',b'T',b'I']
+            NC = 0
+            while True: 
+                c = f.read(1)
+                if c == b'':
+                    break
+                if c == TAG[NC]:
+                    NC+=1
+                    if NC >= len(TAG):
+                        # we found one
+                        l = 0
+                        n = f.read(1)
+                        while n >= b'0' and n<= b'9':
+                            l = (l * 10) + int(n)
+                            n = f.read(1)
+                        NS = (n + f.read(l-1)).decode("ascii")
+                        if NS != "StratusExtensions" and NS != "dsp" and not NS in namespaces:
+                            namespaces.append(NS)
+                        NC = 0
+                else:
+                    NC = 0
+        namespaces.append("dsp")
+        return namespaces
+
     def __init__(self,so_file):
+
         lib = CDLL(so_file)
+
+        self.lib = lib
         self.create = lib.create
         try:
             self.getExtensions = lib.getExtensions
         except:
             self.getExtensions = None
 
+        self.nameSpaces = self._find_namespaces(so_file)
+
         #
         # Using StratusExtensions
         #
         if self.getExtensions is not None:
             self.stratusGetEffectId = getattr(lib,"_ZN17StratusExtensions11getEffectIdEv")
             self.stratusGetName = getattr(lib,"_ZN17StratusExtensions7getNameEv")
             self.stratusGetVersion = getattr(lib,"_ZN17StratusExtensions10getVersionEv")
@@ -28,22 +81,22 @@
             self.stratusGetVersion = None
             self.stratusGetKnobCount = None
             self.stratusGetSwitchCount = None
 
         #
         # Using the effect
         #
-        self.stratusSetKnob = getattr(lib,"_ZN3dsp7setKnobEif")
-        self.stratusGetKnob = getattr(lib,"_ZN3dsp7getKnobEi")
-        self.stratusSetSwitch = getattr(lib,"_ZN3dsp9setSwitchEiNS_12SWITCH_STATEE")
-        self.stratusGetSwitch = getattr(lib,"_ZN3dsp9getSwitchEi")
-        self.stratusSetStompSwitch = getattr(lib,"_ZN3dsp14setStompSwitchENS_12SWITCH_STATEE")
-        self.stratusGetStompSwitch = getattr(lib,"_ZN3dsp14getStompSwitchEv")
-        self.stratusStompSwitchPressed = getattr(lib,"_ZN3dsp18stompSwitchPressedEiPfS0_")
-        self.stratusCompute = getattr(lib,"_ZN3dsp7computeEiPfS0_")
+        self.stratusSetKnob = self._find_func("setKnob","Eif")
+        self.stratusGetKnob = self._find_func("getKnob","Ei")
+        self.stratusSetSwitch = self._find_func("setSwitch","EiNS_12SWITCH_STATEE")
+        self.stratusGetSwitch = self._find_func("getSwitch","Ei")
+        self.stratusSetStompSwitch = self._find_func("setStompSwitch","ENS_12SWITCH_STATEE")
+        self.stratusGetStompSwitch = self._find_func("getStompSwitch","Ev")
+        self.stratusStompSwitchPressed = self._find_func("stompSwitchPressed","EiPfS0_")
+        self.stratusCompute = self._find_func("compute","EiPfS0_")
 
         self.create.restype = InstanceHandle
         if self.getExtensions is not None:
             self.getExtensions.argtypes = [ InstanceHandle ]
             self.getExtensions.restype = InstanceHandle
 
             self.stratusGetEffectId.argtypes = [InstanceHandle]
@@ -57,50 +110,65 @@
 
             self.stratusGetKnobCount.argtypes = [InstanceHandle]
             self.stratusGetKnobCount.restype= c_uint
 
             self.stratusGetSwitchCount.argtypes = [InstanceHandle]
             self.stratusGetSwitchCount.restype= c_uint
 
-        self.stratusSetKnob.argtypes = [InstanceHandle, c_uint, c_float]
-
-        self.stratusGetKnob.argtypes = [InstanceHandle, c_uint]
-        self.stratusGetKnob.restype = c_float
-
-        self.stratusSetSwitch.argtypes = [InstanceHandle, c_uint, c_uint]
-
-        self.stratusGetSwitch.argtypes = [InstanceHandle, c_uint]
-        self.stratusGetSwitch.restype= c_uint
-
-        self.stratusSetStompSwitch.argtypes = [InstanceHandle, c_uint]
-
-        self.stratusGetStompSwitch.argtypes = [InstanceHandle]
-        self.stratusGetStompSwitch.restype = c_uint
+        if self.stratusSetKnob is not None:
+            self.stratusSetKnob.argtypes = [InstanceHandle, c_uint, c_float]
 
-        self.stratusStompSwitchPressed.argtypes = [InstanceHandle, c_uint, FloatPointer, FloatPointer]
-        self.stratusCompute.argtypes = [InstanceHandle, c_uint, FloatPointer, FloatPointer]
+        if self.stratusGetKnob is not None:
+            self.stratusGetKnob.argtypes = [InstanceHandle, c_uint]
+            self.stratusGetKnob.restype = c_float
+
+        if self.stratusSetSwitch is not None:
+            self.stratusSetSwitch.argtypes = [InstanceHandle, c_uint, c_uint]
+
+        if self.stratusGetSwitch is not None:
+            self.stratusGetSwitch.argtypes = [InstanceHandle, c_uint]
+            self.stratusGetSwitch.restype= c_uint
+
+        if self.stratusSetStompSwitch is not None:
+            self.stratusSetStompSwitch.argtypes = [InstanceHandle, c_uint]
+
+        if self.stratusGetStompSwitch is not None:
+            self.stratusGetStompSwitch.argtypes = [InstanceHandle]
+            self.stratusGetStompSwitch.restype = c_uint
+
+        if self.stratusCompute is not None:
+            self.stratusCompute.argtypes = [InstanceHandle, c_uint, FloatPointer, FloatPointer]
+            self.stratusCompute.argtypes = [InstanceHandle, c_uint, FloatPointer, FloatPointer]
 
 
 class Effect:
     """A class that allows a Python script to interact with a Chaos Stratus effect library
 
     Chaos Audio Stratus pedal effects libraries are standard binary shared libraries that 
-    implement a specific interface. Faust - the DSP design system - has a tight integration
-    with such effects. While it is not necessary to design or build effects with Faust, if
-    they are at least built with the same wrapper interface used by the Faust DSP system, then 
-    they are compatible with this class.
+    implement a specific interface. Given an effect library file, this module does all that
+    it can to find the function symbols in the library that represent the implementations of 
+    that interface and thus provide a Python wrapper to the library to allow you to test the
+    library outside of the constraints of the Stratus pedal itself.
+
+    All effects that are built using the Faust integration for the Chaos Stratus are compatible
+    with this module. In addition, effects not built using Faust (including those built before
+    the Faust integration was available) should be "compatible enough" with the wrapper to be
+    usable - they may not implement the StratusExtensions interface that provides useful information
+    such as number of knobs and switches or what have you, but they do implement the basic
+    functional interface, and this module does its level best to find that implementation in the 
+    shared library.
 
-    Note also that the effect has to be built for the system upon which your python script isd
+    Note that the effect has to be built for the system upon which your python script isd
     to run - that means you must either install this package onto your pedal, or you must
     build your effect library for the intended python system.
 
     Again, the Faust tools can help you with this.
 
-    Attributes
-    ----------
+    Attributes (only available through the StratusExtensions interface)
+    -------------------------------------------------------------------
     knobCount : int 
         the number of control knobs the effect uses
     switchCount : int 
         the number of control switches the effect uses
     version : string
         the version of the effect library
     effectId : string
```

### Comparing `chaos_stratus-1.0.1/src/chaos_stratus.egg-info/PKG-INFO` & `chaos_stratus-1.1.0/src/chaos_stratus.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 Metadata-Version: 2.1
 Name: chaos-stratus
-Version: 1.0.1
-Summary: Python tools used to interact with (appropriately compiled) Chaos Stratus effect libraries
+Version: 1.1.0
+Summary: Python tools used to interact with Chaos Stratus effect libraries
 Author-email: Martin Bartlett <martin.j.bartlett@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/bassmanitram/chaos-stratus-python
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.0
+Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 
 
 # chaos-stratus
 
 This package provides tools for interacting with (appropriately compiled) [Chaos Audio Stratus pedal](https://chaosaudio.com/) effects libraries. 
 
-By "appropriately compiled" we mean built with the Stratus build tools available with the most recent versions of [Faust](https://faust.grame.fr/), or with the [Faust IDE](https://faustide.grame.fr/).
+By "appropriately compiled" we mean built with the Stratus build tools available with the most recent versions of [Faust](https://faust.grame.fr/), 
+or with the [Faust IDE](https://faustide.grame.fr/).
+
+Effects that are _not_ built with the Faust tools (e.g. those built before those tools became available) are still at least _partially_ compatible
+with the library - they may not provide the documented class attributes, but they will provide the operational functions that allow you
+to interact with them.
+
+In _all_ cases, though, the effect must be built for the platform upon which this class is used - that means performing a "local" build with the
+Faust tools (or by some other means) or installing this package on the Stratus pedal itself.
 
-(Note that prior to the full Faust integration of the Stratus development tools, effects libraries were built in such a way as to NOT be fully compatible with these tools).
 # Installation
 
 You can install this package using a standard `pip` invocation
 
 
 ```
 python -m pip install chaos-stratus
```

