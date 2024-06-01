# Comparing `tmp/pyarmor.cli.core-6.5.1.zip` & `tmp/pyarmor.cli.core-6.5.2.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 8999 bytes, number of entries: 16
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-19 15:50 pyarmor.cli.core-6.5.1/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-19 15:50 pyarmor.cli.core-6.5.1/pyarmor/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-19 15:50 pyarmor.cli.core-6.5.1/pyarmor.cli.core.egg-info/
--rw-r--r--  2.0 unx     2647 b- defN 24-Apr-19 15:50 pyarmor.cli.core-6.5.1/PKG-INFO
--rw-r--r--  2.0 unx     2033 b- defN 24-Apr-13 10:14 pyarmor.cli.core-6.5.1/setup.py
--rw-r--r--  2.0 unx       38 b- defN 24-Apr-19 15:50 pyarmor.cli.core-6.5.1/setup.cfg
--rw-r--r--  2.0 unx     1548 b- defN 23-Jul-02 16:45 pyarmor.cli.core-6.5.1/README.rst
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-19 15:50 pyarmor.cli.core-6.5.1/pyarmor/cli/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-19 15:50 pyarmor.cli.core-6.5.1/pyarmor/cli/core/
--rw-r--r--  2.0 unx     4647 b- defN 24-Apr-13 10:14 pyarmor.cli.core-6.5.1/pyarmor/cli/core/__init__.py
--rw-r--r--  2.0 unx     1513 b- defN 23-Jun-06 07:58 pyarmor.cli.core-6.5.1/pyarmor/cli/core/features.py
--rw-r--r--  2.0 unx     2798 b- defN 23-Jun-08 15:05 pyarmor.cli.core-6.5.1/pyarmor/cli/core/runtime.py
--rw-r--r--  2.0 unx     2647 b- defN 24-Apr-19 15:50 pyarmor.cli.core-6.5.1/pyarmor.cli.core.egg-info/PKG-INFO
--rw-r--r--  2.0 unx      265 b- defN 24-Apr-19 15:50 pyarmor.cli.core-6.5.1/pyarmor.cli.core.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx        8 b- defN 24-Apr-19 15:50 pyarmor.cli.core-6.5.1/pyarmor.cli.core.egg-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-19 15:50 pyarmor.cli.core-6.5.1/pyarmor.cli.core.egg-info/dependency_links.txt
-16 files, 18145 bytes uncompressed, 6351 bytes compressed:  65.0%
+Zip file size: 9170 bytes, number of entries: 16
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-30 11:02 pyarmor.cli.core-6.5.2/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-30 11:02 pyarmor.cli.core-6.5.2/pyarmor/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-30 11:02 pyarmor.cli.core-6.5.2/pyarmor.cli.core.egg-info/
+-rw-r--r--  2.0 unx     3435 b- defN 24-May-30 11:02 pyarmor.cli.core-6.5.2/PKG-INFO
+-rw-r--r--  2.0 unx     2033 b- defN 24-May-17 18:43 pyarmor.cli.core-6.5.2/setup.py
+-rw-r--r--  2.0 unx       38 b- defN 24-May-30 11:02 pyarmor.cli.core-6.5.2/setup.cfg
+-rw-r--r--  2.0 unx     2200 b- defN 24-May-27 10:22 pyarmor.cli.core-6.5.2/README.rst
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-30 11:02 pyarmor.cli.core-6.5.2/pyarmor/cli/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-30 11:02 pyarmor.cli.core-6.5.2/pyarmor/cli/core/
+-rw-r--r--  2.0 unx     4186 b- defN 24-May-27 20:42 pyarmor.cli.core-6.5.2/pyarmor/cli/core/__init__.py
+-rw-r--r--  2.0 unx     1513 b- defN 23-Jun-06 07:58 pyarmor.cli.core-6.5.2/pyarmor/cli/core/features.py
+-rw-r--r--  2.0 unx     2440 b- defN 24-May-27 12:18 pyarmor.cli.core-6.5.2/pyarmor/cli/core/runtime.py
+-rw-r--r--  2.0 unx     3435 b- defN 24-May-30 11:02 pyarmor.cli.core-6.5.2/pyarmor.cli.core.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx      265 b- defN 24-May-30 11:02 pyarmor.cli.core-6.5.2/pyarmor.cli.core.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx        8 b- defN 24-May-30 11:02 pyarmor.cli.core-6.5.2/pyarmor.cli.core.egg-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-May-30 11:02 pyarmor.cli.core-6.5.2/pyarmor.cli.core.egg-info/dependency_links.txt
+16 files, 19554 bytes uncompressed, 6522 bytes compressed:  66.6%
```

## zipnote {}

```diff
@@ -1,49 +1,49 @@
-Filename: pyarmor.cli.core-6.5.1/
+Filename: pyarmor.cli.core-6.5.2/
 Comment: 
 
-Filename: pyarmor.cli.core-6.5.1/pyarmor/
+Filename: pyarmor.cli.core-6.5.2/pyarmor/
 Comment: 
 
-Filename: pyarmor.cli.core-6.5.1/pyarmor.cli.core.egg-info/
+Filename: pyarmor.cli.core-6.5.2/pyarmor.cli.core.egg-info/
 Comment: 
 
-Filename: pyarmor.cli.core-6.5.1/PKG-INFO
+Filename: pyarmor.cli.core-6.5.2/PKG-INFO
 Comment: 
 
-Filename: pyarmor.cli.core-6.5.1/setup.py
+Filename: pyarmor.cli.core-6.5.2/setup.py
 Comment: 
 
-Filename: pyarmor.cli.core-6.5.1/setup.cfg
+Filename: pyarmor.cli.core-6.5.2/setup.cfg
 Comment: 
 
-Filename: pyarmor.cli.core-6.5.1/README.rst
+Filename: pyarmor.cli.core-6.5.2/README.rst
 Comment: 
 
-Filename: pyarmor.cli.core-6.5.1/pyarmor/cli/
+Filename: pyarmor.cli.core-6.5.2/pyarmor/cli/
 Comment: 
 
-Filename: pyarmor.cli.core-6.5.1/pyarmor/cli/core/
+Filename: pyarmor.cli.core-6.5.2/pyarmor/cli/core/
 Comment: 
 
-Filename: pyarmor.cli.core-6.5.1/pyarmor/cli/core/__init__.py
+Filename: pyarmor.cli.core-6.5.2/pyarmor/cli/core/__init__.py
 Comment: 
 
-Filename: pyarmor.cli.core-6.5.1/pyarmor/cli/core/features.py
+Filename: pyarmor.cli.core-6.5.2/pyarmor/cli/core/features.py
 Comment: 
 
-Filename: pyarmor.cli.core-6.5.1/pyarmor/cli/core/runtime.py
+Filename: pyarmor.cli.core-6.5.2/pyarmor/cli/core/runtime.py
 Comment: 
 
-Filename: pyarmor.cli.core-6.5.1/pyarmor.cli.core.egg-info/PKG-INFO
+Filename: pyarmor.cli.core-6.5.2/pyarmor.cli.core.egg-info/PKG-INFO
 Comment: 
 
-Filename: pyarmor.cli.core-6.5.1/pyarmor.cli.core.egg-info/SOURCES.txt
+Filename: pyarmor.cli.core-6.5.2/pyarmor.cli.core.egg-info/SOURCES.txt
 Comment: 
 
-Filename: pyarmor.cli.core-6.5.1/pyarmor.cli.core.egg-info/top_level.txt
+Filename: pyarmor.cli.core-6.5.2/pyarmor.cli.core.egg-info/top_level.txt
 Comment: 
 
-Filename: pyarmor.cli.core-6.5.1/pyarmor.cli.core.egg-info/dependency_links.txt
+Filename: pyarmor.cli.core-6.5.2/pyarmor.cli.core.egg-info/dependency_links.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `pyarmor.cli.core-6.5.1/setup.py` & `pyarmor.cli.core-6.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
 from setuptools import setup
 
-__VERSION__ = '6.5.1'
+__VERSION__ = '6.5.2'
 
 with open('README.rst') as f:
     long_description = f.read()
 
 is_android = hasattr(sys, 'getandroidapilevel')
 is_freebsd = sys.platform.startswith(('freebsd', 'openbsd', 'isilon onefs'))
```

## Comparing `pyarmor.cli.core-6.5.1/pyarmor/cli/core/__init__.py` & `pyarmor.cli.core-6.5.2/pyarmor/cli/core/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,75 +16,58 @@
 #  @File: pyarmor/core/__init__.py
 #
 #  @Author: Jondy Zhao (pyarmor@163.com)
 #
 #  @Create Date: Thu Jan 12 17:29:25 CST 2023
 #
 
-__VERSION__ = '6.5.1'
+__VERSION__ = '6.5.2'
 
+PLATFORM_NAMES = (
+    'windows.x86_64', 'windows.x86',
+    'darwin.x86_64', 'darwin.arm64',
+    'linux.x86_64', 'linux.x86', 'linux.aarch64', 'linux.armv7',
+    'linux.mips32el', 'linux.mips64el', 'linux.ppc64le', 'linux.riscv64',
+    'alpine.x86_64', 'alpine.aarch64',
+    'alpine.mips32el', 'alpine.mips64el', 'alpine.ppc64le', 'alpine.riscv64',
+    'freebsd.x86_64',
+    'android.x86_64', 'android.x86', 'android.aarch64', 'android.armv7',
+)
+
+
+def map_platform(platname):
+    if platname == 'darwin.aarch64':
+        return 'darwin.arm64'
+    return platname
+
+
+def check_and_install_prebuilt_package():
+    import os
+    from pyarmor.cli.context import format_platform
+    from pyarmor.cli.bootstrap import check_prebuilt_runtime_library
+
+    plat, arch = format_platform()
+    platname = map_platform('%s.%s' % (plat, arch))
+    if platname not in PLATFORM_NAMES:
+        raise RuntimeError('"%s" is still not supported by Pyarmor' % platname)
 
-def format_platform():
-    import platform
-    import sys
-    from struct import calcsize
-
-    def format_system():
-        plat = platform.system().lower()
-        plat = ('windows' if plat.startswith('cygwin') else
-                'linux' if plat.startswith('linux') else
-                'freebsd' if plat.startswith(
-                    ('freebsd', 'openbsd', 'isilon onefs')) else plat)
-        if plat == 'linux':
-            if hasattr(sys, 'getandroidapilevel'):
-                plat = 'android'
-            else:
-                cname, cver = platform.libc_ver()
-                if cname == 'musl':
-                    plat = 'alpine'
-                elif cname == 'libc':
-                    plat = 'android'
-        return plat
-
-    def format_machine():
-        mach = platform.machine().lower()
-        arch_table = (
-            ('x86', ('i386', 'i486', 'i586', 'i686')),
-            ('x86_64', ('x64', 'x86_64', 'amd64', 'intel')),
-            ('arm', ('armv5',)),
-            ('armv6', ('armv6l',)),
-            ('armv7', ('armv7l',)),
-            ('aarch32', ('aarch32',)),
-            ('aarch64', ('aarch64', 'arm64'))
-        )
-        for alias, archlist in arch_table:
-            if mach in archlist:
-                mach = alias
-                break
-        return mach
-
-    plat, mach = format_system(), format_machine()
-    if plat == 'windows' and mach == 'x86_64':
-        bitness = calcsize('P'.encode()) * 8
-        if bitness == 32:
-            mach = 'x86'
-    elif plat == 'darwin' and mach == 'aarch64':
-        mach = 'arm64'
+    if not os.path.exists(os.path.join(os.path.dirname(__file__), plat, arch)):
+        check_prebuilt_runtime_library([platname])
 
-    return plat, mach
+    return plat, arch
 
 
 def _import_pytransform3():
     try:
         return __import__(
             'pytransform3', globals=globals(), locals=locals(),
             fromlist=('__pyarmor__',), level=1
         )
     except ModuleNotFoundError:
-        plat, arch = format_platform()
+        plat, arch = check_and_install_prebuilt_package()
         modname = '.'.join([plat, arch, 'pytransform3'])
         return __import__(
             modname, globals=globals(), locals=locals(),
             fromlist=('__pyarmor__',), level=1
         )
```

## Comparing `pyarmor.cli.core-6.5.1/pyarmor/cli/core/features.py` & `pyarmor.cli.core-6.5.2/pyarmor/cli/core/features.py`

 * *Files identical despite different names*

## Comparing `pyarmor.cli.core-6.5.1/pyarmor/cli/core/runtime.py` & `pyarmor.cli.core-6.5.2/pyarmor/cli/core/runtime.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,28 +16,15 @@
 #  @File: pyarmor/core/runtime.py
 #
 #  @Author: Jondy Zhao (pyarmor@163.com)
 #
 #  @Create Date: Tue Jun  6 07:50:00 CST 2023
 #
 
-PLATFORM_NAMES = (
-    'windows.x86_64', 'windows.x86',
-    'darwin.x86_64', 'darwin.arm64',
-    'linux.x86_64', 'linux.x86', 'linux.aarch64', 'linux.armv7',
-    'alpine.x86_64', 'alpine.aarch64',
-    'freebsd.x86_64',
-    'android.x86_64', 'android.x86', 'android.aarch64', 'android.armv7',
-)
-
-
-def map_platform(platname):
-    if platname == 'darwin.aarch64':
-        return 'darwin.arm64'
-    return platname
+from . import map_platform
 
 
 class PyarmorRuntime(object):
 
     @staticmethod
     def get(plat, extra=None, native=True):
         from os import scandir, path as os_path
@@ -51,19 +38,20 @@
         if native and not extra:
             path = pkgpath
             for entry in scandir(path):
                 parts = entry.name.split('.')
                 if parts[0] == prefix and parts[-1] in ('so', 'pyd', 'dylib'):
                     return entry.name, os_path.abspath(entry.path)
 
-        dirnames = map_platform(plat).split('.')
+        platname = map_platform(plat)
+        dirnames = platname.split('.')
         path = os_path.join(pkgpath, extra if extra else '', *dirnames)
         if not os_path.exists(path):
             from pyarmor.cli.bootstrap import check_prebuilt_runtime_library
-            check_prebuilt_runtime_library(dirnames[:1], extra)
+            check_prebuilt_runtime_library([platname], extra)
 
         if os_path.exists(path):
             for entry in scandir(path):
                 parts = entry.name.split('.')
                 if parts[0] == prefix and parts[-1] in ('so', 'pyd', 'dylib'):
                     return entry.name, os_path.abspath(entry.path)
```

