# Comparing `tmp/WinDirectInput-1.2.1.tar.gz` & `tmp/WinDirectInput-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WinDirectInput-1.2.1.tar", last modified: Sat Jun  1 10:13:37 2024, max compression
+gzip compressed data, was "WinDirectInput-1.2.3.tar", last modified: Sat Jun  1 11:57:35 2024, max compression
```

## Comparing `WinDirectInput-1.2.1.tar` & `WinDirectInput-1.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 10:13:37.287540 WinDirectInput-1.2.1/
--rw-rw-rw-   0        0        0     1093 2024-02-02 06:02:27.000000 WinDirectInput-1.2.1/LICENSE
--rw-rw-rw-   0        0        0     9228 2024-06-01 10:13:37.286539 WinDirectInput-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     8524 2024-06-01 10:07:14.000000 WinDirectInput-1.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-06-01 10:13:37.285542 WinDirectInput-1.2.1/WinDirectInput.egg-info/
--rw-rw-rw-   0        0        0     9228 2024-06-01 10:13:37.000000 WinDirectInput-1.2.1/WinDirectInput.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2024-06-01 10:13:37.000000 WinDirectInput-1.2.1/WinDirectInput.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 10:13:37.000000 WinDirectInput-1.2.1/WinDirectInput.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-06-01 10:13:37.000000 WinDirectInput-1.2.1/WinDirectInput.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-06-01 10:13:37.000000 WinDirectInput-1.2.1/WinDirectInput.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    44175 2024-06-01 09:35:59.000000 WinDirectInput-1.2.1/directinput.py
--rw-rw-rw-   0        0        0       42 2024-06-01 10:13:37.287540 WinDirectInput-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0      876 2024-06-01 10:04:49.000000 WinDirectInput-1.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-06-01 10:13:37.285542 WinDirectInput-1.2.1/tests/
--rw-rw-rw-   0        0        0      118 2024-05-15 12:48:24.000000 WinDirectInput-1.2.1/tests/test.py
+drwxrwxrwx   0        0        0        0 2024-06-01 11:57:35.563691 WinDirectInput-1.2.3/
+-rw-rw-rw-   0        0        0     1093 2024-02-02 06:02:27.000000 WinDirectInput-1.2.3/LICENSE
+-rw-rw-rw-   0        0        0     9229 2024-06-01 11:57:35.562691 WinDirectInput-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     8525 2024-06-01 11:48:28.000000 WinDirectInput-1.2.3/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 11:57:35.561687 WinDirectInput-1.2.3/WinDirectInput.egg-info/
+-rw-rw-rw-   0        0        0     9229 2024-06-01 11:57:35.000000 WinDirectInput-1.2.3/WinDirectInput.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2024-06-01 11:57:35.000000 WinDirectInput-1.2.3/WinDirectInput.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 11:57:35.000000 WinDirectInput-1.2.3/WinDirectInput.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-06-01 11:57:35.000000 WinDirectInput-1.2.3/WinDirectInput.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-06-01 11:57:35.000000 WinDirectInput-1.2.3/WinDirectInput.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    44175 2024-06-01 09:35:59.000000 WinDirectInput-1.2.3/directinput.py
+-rw-rw-rw-   0        0        0       42 2024-06-01 11:57:35.563691 WinDirectInput-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      876 2024-06-01 11:57:29.000000 WinDirectInput-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 11:57:35.561687 WinDirectInput-1.2.3/tests/
+-rw-rw-rw-   0        0        0      118 2024-05-15 12:48:24.000000 WinDirectInput-1.2.3/tests/test.py
```

### Comparing `WinDirectInput-1.2.1/LICENSE` & `WinDirectInput-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `WinDirectInput-1.2.1/PKG-INFO` & `WinDirectInput-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WinDirectInput
-Version: 1.2.1
+Version: 1.2.3
 Summary: A Windows-specific package for simulating keyboard and mouse inputs
 Home-page: https://github.com/abdulrahimpds/WinDirectInput
 Author: AbdulRahim Khan
 Author-email: abdulrahimpds@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -89,15 +89,15 @@
 - **Function Keys**: 
   - `f1`, `f2`, `f3`, `f4`, `f5`, `f6`, `f7`, `f8`, `f9`, `f10`, `f11`, `f12`
 
 - **Control Keys**:
   - `space`, `esc`, `tab`, `backspace`, `enter`, `numenter`, `shift`, `lshift`, `rshift`, `ctrl`, `lctrl`, `rctrl`, `alt`, `lalt`, `ralt`, `win`, `lwin`, `rwin`, `apps`, `capslock`, `numlock`, `scrolllock`, `insert`, `delete`, `home`, `end`, `pageup`, `pagedown`, `prtsc`, `sysrq`
 
 - **Calculation Keys**:
-  -`num-`, `num/`, `num*`, `num+`, `num.`
+  - `num-`, `num/`, `num*`, `num+`, `num.`
 
 - **Arrow Keys**: 
   - `up`, `down`, `left`, `right`
 
 ### Mouse Buttons
 
 - **Primary Buttons**:
```

### Comparing `WinDirectInput-1.2.1/README.md` & `WinDirectInput-1.2.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 - **Function Keys**: 
   - `f1`, `f2`, `f3`, `f4`, `f5`, `f6`, `f7`, `f8`, `f9`, `f10`, `f11`, `f12`
 
 - **Control Keys**:
   - `space`, `esc`, `tab`, `backspace`, `enter`, `numenter`, `shift`, `lshift`, `rshift`, `ctrl`, `lctrl`, `rctrl`, `alt`, `lalt`, `ralt`, `win`, `lwin`, `rwin`, `apps`, `capslock`, `numlock`, `scrolllock`, `insert`, `delete`, `home`, `end`, `pageup`, `pagedown`, `prtsc`, `sysrq`
 
 - **Calculation Keys**:
-  -`num-`, `num/`, `num*`, `num+`, `num.`
+  - `num-`, `num/`, `num*`, `num+`, `num.`
 
 - **Arrow Keys**: 
   - `up`, `down`, `left`, `right`
 
 ### Mouse Buttons
 
 - **Primary Buttons**:
```

### Comparing `WinDirectInput-1.2.1/WinDirectInput.egg-info/PKG-INFO` & `WinDirectInput-1.2.3/WinDirectInput.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WinDirectInput
-Version: 1.2.1
+Version: 1.2.3
 Summary: A Windows-specific package for simulating keyboard and mouse inputs
 Home-page: https://github.com/abdulrahimpds/WinDirectInput
 Author: AbdulRahim Khan
 Author-email: abdulrahimpds@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -89,15 +89,15 @@
 - **Function Keys**: 
   - `f1`, `f2`, `f3`, `f4`, `f5`, `f6`, `f7`, `f8`, `f9`, `f10`, `f11`, `f12`
 
 - **Control Keys**:
   - `space`, `esc`, `tab`, `backspace`, `enter`, `numenter`, `shift`, `lshift`, `rshift`, `ctrl`, `lctrl`, `rctrl`, `alt`, `lalt`, `ralt`, `win`, `lwin`, `rwin`, `apps`, `capslock`, `numlock`, `scrolllock`, `insert`, `delete`, `home`, `end`, `pageup`, `pagedown`, `prtsc`, `sysrq`
 
 - **Calculation Keys**:
-  -`num-`, `num/`, `num*`, `num+`, `num.`
+  - `num-`, `num/`, `num*`, `num+`, `num.`
 
 - **Arrow Keys**: 
   - `up`, `down`, `left`, `right`
 
 ### Mouse Buttons
 
 - **Primary Buttons**:
```

### Comparing `WinDirectInput-1.2.1/directinput.py` & `WinDirectInput-1.2.3/directinput.py`

 * *Files identical despite different names*

### Comparing `WinDirectInput-1.2.1/setup.py` & `WinDirectInput-1.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='WinDirectInput',
-    version='1.2.1',
+    version='1.2.3',
     author='AbdulRahim Khan',
     author_email='abdulrahimpds@gmail.com',
     description='A Windows-specific package for simulating keyboard and mouse inputs',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/abdulrahimpds/WinDirectInput',
     py_modules=['directinput'],
```

