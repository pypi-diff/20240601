# Comparing `tmp/WinDirectInput-1.1.0.tar.gz` & `tmp/WinDirectInput-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WinDirectInput-1.1.0.tar", last modified: Wed May 15 14:47:10 2024, max compression
+gzip compressed data, was "WinDirectInput-1.2.0.tar", last modified: Sat Jun  1 10:00:32 2024, max compression
```

## Comparing `WinDirectInput-1.1.0.tar` & `WinDirectInput-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 14:47:10.571281 WinDirectInput-1.1.0/
--rw-rw-rw-   0        0        0     1093 2024-02-02 06:02:27.000000 WinDirectInput-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     7553 2024-05-15 14:47:10.570281 WinDirectInput-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     6849 2024-05-15 14:46:35.000000 WinDirectInput-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 14:47:10.569278 WinDirectInput-1.1.0/WinDirectInput.egg-info/
--rw-rw-rw-   0        0        0     7553 2024-05-15 14:47:10.000000 WinDirectInput-1.1.0/WinDirectInput.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2024-05-15 14:47:10.000000 WinDirectInput-1.1.0/WinDirectInput.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 14:47:10.000000 WinDirectInput-1.1.0/WinDirectInput.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-05-15 14:47:10.000000 WinDirectInput-1.1.0/WinDirectInput.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-15 14:47:10.000000 WinDirectInput-1.1.0/WinDirectInput.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    43793 2024-05-15 14:38:13.000000 WinDirectInput-1.1.0/directinput.py
--rw-rw-rw-   0        0        0       42 2024-05-15 14:47:10.571281 WinDirectInput-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      876 2024-05-15 12:32:05.000000 WinDirectInput-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-15 14:47:10.568273 WinDirectInput-1.1.0/tests/
--rw-rw-rw-   0        0        0      118 2024-05-15 12:48:24.000000 WinDirectInput-1.1.0/tests/test.py
+drwxrwxrwx   0        0        0        0 2024-06-01 10:00:32.501654 WinDirectInput-1.2.0/
+-rw-rw-rw-   0        0        0     1093 2024-02-02 06:02:27.000000 WinDirectInput-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     9158 2024-06-01 10:00:32.500644 WinDirectInput-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8454 2024-06-01 09:55:45.000000 WinDirectInput-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 10:00:32.499654 WinDirectInput-1.2.0/WinDirectInput.egg-info/
+-rw-rw-rw-   0        0        0     9158 2024-06-01 10:00:32.000000 WinDirectInput-1.2.0/WinDirectInput.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2024-06-01 10:00:32.000000 WinDirectInput-1.2.0/WinDirectInput.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 10:00:32.000000 WinDirectInput-1.2.0/WinDirectInput.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-06-01 10:00:32.000000 WinDirectInput-1.2.0/WinDirectInput.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-06-01 10:00:32.000000 WinDirectInput-1.2.0/WinDirectInput.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    44175 2024-06-01 09:35:59.000000 WinDirectInput-1.2.0/directinput.py
+-rw-rw-rw-   0        0        0       42 2024-06-01 10:00:32.501654 WinDirectInput-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      876 2024-06-01 09:58:16.000000 WinDirectInput-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 10:00:32.498653 WinDirectInput-1.2.0/tests/
+-rw-rw-rw-   0        0        0      118 2024-05-15 12:48:24.000000 WinDirectInput-1.2.0/tests/test.py
```

### Comparing `WinDirectInput-1.1.0/LICENSE` & `WinDirectInput-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `WinDirectInput-1.1.0/PKG-INFO` & `WinDirectInput-1.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WinDirectInput
-Version: 1.1.0
+Version: 1.2.0
 Summary: A Windows-specific package for simulating keyboard and mouse inputs
 Home-page: https://github.com/abdulrahimpds/WinDirectInput
 Author: AbdulRahim Khan
 Author-email: abdulrahimpds@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -66,35 +66,72 @@
 - `moveMouse(xOffset=int/float, yOffset=int/float, duration=int/float)`: Moves the mouse cursor relative to its current position by specified x and y offsets over a specified duration.
 - `scrollMouse(clicks=int)`: Scrolls the mouse wheel vertically. The `clicks` parameter determines the amount and direction of the scroll: a positive value scrolls up, while a negative value scrolls down. For a visible result, it is recommended to use a value of 100 or more, as smaller numbers may not produce a significant scrolling.
 - `screenshot(filename=str, region=tuple)`: Takes a screenshot of the entire screen. Additionally, there's a `region` parameter which captures specified region of the screen. It takes a tuple specifying the top-left x, top-left y, width, and height.
 - `getMousePosition()`: Returns the current (x, y) position of the mouse cursor.
 - `getDisplaySize()`
 - `locateImage(needleImage=str, haystackImage=str, grayscale=bool, region=tuple, threshold=float)`: Searches for an image (`needleImage`) within another image (`haystackImage`) or the screen. If `haystackImage` is not provided, the entire screen is used. The `grayscale` parameter can be set to `True` to perform the search in grayscale, which can improve performance. The `region` parameter can specify a specific area to search within, and `threshold` sets the accuracy required for a match.
 
+## Available Keys and Mouse Buttons
+
+All the keys listed can be detected as well as pressed, except `xbutton1` and `xbutton2`, which cannot be pressed.
+
+### Keyboard Keys
+
+- **Alphabets**: 
+  - `a`, `A`, `b`, `B`, `c`, `C`, `d`, `D`, `e`, `E`, `f`, `F`, `g`, `G`, `h`, `H`, `i`, `I`, `j`, `J`, `k`, `K`, `l`, `L`, `m`, `M`, `n`, `N`, `o`, `O`, `p`, `P`, `q`, `Q`, `r`, `R`, `s`, `S`, `t`, `T`, `u`, `U`, `v`, `V`, `w`, `W`, `x`, `X`, `y`, `Y`, `z`, `Z`
+
+- **Numbers**: 
+  - `0`, `1`, `2`, `3`, `4`, `5`, `6`, `7`, `8`, `9`
+  - `num0`, `num1`, `num2`, `num3`, `num4`, `num5`, `num6`, `num7`, `num8`, `num9`
+
+- **Symbols**:
+  - `` ` ``, `~`, `!`, `@`, `#`, `$`, `%`, `^`, `&`, `*`, `(`, `)`, `-`, `_`, `=`, `+`, `[`, `{`, `]`, `}`, `\`, `|`, `;`, `:`, `'`, `"`, `,`, `<`, `.`, `>`, `/`, `?`
+
+- **Function Keys**: 
+  - `f1`, `f2`, `f3`, `f4`, `f5`, `f6`, `f7`, `f8`, `f9`, `f10`, `f11`, `f12`
+
+- **Control Keys**:
+  - `space`, `esc`, `tab`, `backspace`, `enter`, `numenter`, `shift`, `lshift`, `rshift`, `ctrl`, `lctrl`, `rctrl`, `alt`, `lalt`, `ralt`, `win`, `lwin`, `rwin`, `apps`, `capslock`, `numlock`, `scrolllock`, `insert`, `delete`, `home`, `end`, `pageup`, `pagedown`, `prtsc`, `sysrq`
+
+- **Arrow Keys**: 
+  - `up`, `down`, `left`, `right`
+
+### Mouse Buttons
+
+- **Primary Buttons**: 
+  - `left`, `right`, `middle`
+
+- **Additional Buttons**: 
+  - `xbutton1` (can only be detected), `xbutton2` (can only be detected)
+
 ## Example Usage
 
 ### Writing Complex Strings
 
 ```Python
 import directinput
 
 # Writing a string with special characters
-directinput.write("Hello, world!")
+directinput.write("Hello, world! ✌️")
 ```
 
 This demonstrates the enhanced write function, capable of handling a wide range of characters, surpassing limitations you might find in other modules.
 
 ### Detecting Key Presses
 
 ```Python
 import directinput
 
 # Detect if the 'A' key is being pressed
 if directinput.keyDetect('a'):
     print("The 'A' key is pressed!")
+
+# Detect if both 'left_mouse' and 'xbutton1' is being pressed
+if directinput.keyDetect(['left_mouse', 'xbutton1']):
+    print("Pressed!")
 ```
 
 ### Locating an Image on the Screen
 
 The locateImage function in WinDirectInput adds a layer of flexibility to image detection. Whether you're automating tasks based on visual cues or integrating with image processing, this function is incredibly handy.
 
 ```Python
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `WinDirectInput-1.1.0/README.md` & `WinDirectInput-1.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -45,35 +45,72 @@
 - `moveMouse(xOffset=int/float, yOffset=int/float, duration=int/float)`: Moves the mouse cursor relative to its current position by specified x and y offsets over a specified duration.
 - `scrollMouse(clicks=int)`: Scrolls the mouse wheel vertically. The `clicks` parameter determines the amount and direction of the scroll: a positive value scrolls up, while a negative value scrolls down. For a visible result, it is recommended to use a value of 100 or more, as smaller numbers may not produce a significant scrolling.
 - `screenshot(filename=str, region=tuple)`: Takes a screenshot of the entire screen. Additionally, there's a `region` parameter which captures specified region of the screen. It takes a tuple specifying the top-left x, top-left y, width, and height.
 - `getMousePosition()`: Returns the current (x, y) position of the mouse cursor.
 - `getDisplaySize()`
 - `locateImage(needleImage=str, haystackImage=str, grayscale=bool, region=tuple, threshold=float)`: Searches for an image (`needleImage`) within another image (`haystackImage`) or the screen. If `haystackImage` is not provided, the entire screen is used. The `grayscale` parameter can be set to `True` to perform the search in grayscale, which can improve performance. The `region` parameter can specify a specific area to search within, and `threshold` sets the accuracy required for a match.
 
+## Available Keys and Mouse Buttons
+
+All the keys listed can be detected as well as pressed, except `xbutton1` and `xbutton2`, which cannot be pressed.
+
+### Keyboard Keys
+
+- **Alphabets**: 
+  - `a`, `A`, `b`, `B`, `c`, `C`, `d`, `D`, `e`, `E`, `f`, `F`, `g`, `G`, `h`, `H`, `i`, `I`, `j`, `J`, `k`, `K`, `l`, `L`, `m`, `M`, `n`, `N`, `o`, `O`, `p`, `P`, `q`, `Q`, `r`, `R`, `s`, `S`, `t`, `T`, `u`, `U`, `v`, `V`, `w`, `W`, `x`, `X`, `y`, `Y`, `z`, `Z`
+
+- **Numbers**: 
+  - `0`, `1`, `2`, `3`, `4`, `5`, `6`, `7`, `8`, `9`
+  - `num0`, `num1`, `num2`, `num3`, `num4`, `num5`, `num6`, `num7`, `num8`, `num9`
+
+- **Symbols**:
+  - `` ` ``, `~`, `!`, `@`, `#`, `$`, `%`, `^`, `&`, `*`, `(`, `)`, `-`, `_`, `=`, `+`, `[`, `{`, `]`, `}`, `\`, `|`, `;`, `:`, `'`, `"`, `,`, `<`, `.`, `>`, `/`, `?`
+
+- **Function Keys**: 
+  - `f1`, `f2`, `f3`, `f4`, `f5`, `f6`, `f7`, `f8`, `f9`, `f10`, `f11`, `f12`
+
+- **Control Keys**:
+  - `space`, `esc`, `tab`, `backspace`, `enter`, `numenter`, `shift`, `lshift`, `rshift`, `ctrl`, `lctrl`, `rctrl`, `alt`, `lalt`, `ralt`, `win`, `lwin`, `rwin`, `apps`, `capslock`, `numlock`, `scrolllock`, `insert`, `delete`, `home`, `end`, `pageup`, `pagedown`, `prtsc`, `sysrq`
+
+- **Arrow Keys**: 
+  - `up`, `down`, `left`, `right`
+
+### Mouse Buttons
+
+- **Primary Buttons**: 
+  - `left`, `right`, `middle`
+
+- **Additional Buttons**: 
+  - `xbutton1` (can only be detected), `xbutton2` (can only be detected)
+
 ## Example Usage
 
 ### Writing Complex Strings
 
 ```Python
 import directinput
 
 # Writing a string with special characters
-directinput.write("Hello, world!")
+directinput.write("Hello, world! ✌️")
 ```
 
 This demonstrates the enhanced write function, capable of handling a wide range of characters, surpassing limitations you might find in other modules.
 
 ### Detecting Key Presses
 
 ```Python
 import directinput
 
 # Detect if the 'A' key is being pressed
 if directinput.keyDetect('a'):
     print("The 'A' key is pressed!")
+
+# Detect if both 'left_mouse' and 'xbutton1' is being pressed
+if directinput.keyDetect(['left_mouse', 'xbutton1']):
+    print("Pressed!")
 ```
 
 ### Locating an Image on the Screen
 
 The locateImage function in WinDirectInput adds a layer of flexibility to image detection. Whether you're automating tasks based on visual cues or integrating with image processing, this function is incredibly handy.
 
 ```Python
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `WinDirectInput-1.1.0/WinDirectInput.egg-info/PKG-INFO` & `WinDirectInput-1.2.0/WinDirectInput.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WinDirectInput
-Version: 1.1.0
+Version: 1.2.0
 Summary: A Windows-specific package for simulating keyboard and mouse inputs
 Home-page: https://github.com/abdulrahimpds/WinDirectInput
 Author: AbdulRahim Khan
 Author-email: abdulrahimpds@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -66,35 +66,72 @@
 - `moveMouse(xOffset=int/float, yOffset=int/float, duration=int/float)`: Moves the mouse cursor relative to its current position by specified x and y offsets over a specified duration.
 - `scrollMouse(clicks=int)`: Scrolls the mouse wheel vertically. The `clicks` parameter determines the amount and direction of the scroll: a positive value scrolls up, while a negative value scrolls down. For a visible result, it is recommended to use a value of 100 or more, as smaller numbers may not produce a significant scrolling.
 - `screenshot(filename=str, region=tuple)`: Takes a screenshot of the entire screen. Additionally, there's a `region` parameter which captures specified region of the screen. It takes a tuple specifying the top-left x, top-left y, width, and height.
 - `getMousePosition()`: Returns the current (x, y) position of the mouse cursor.
 - `getDisplaySize()`
 - `locateImage(needleImage=str, haystackImage=str, grayscale=bool, region=tuple, threshold=float)`: Searches for an image (`needleImage`) within another image (`haystackImage`) or the screen. If `haystackImage` is not provided, the entire screen is used. The `grayscale` parameter can be set to `True` to perform the search in grayscale, which can improve performance. The `region` parameter can specify a specific area to search within, and `threshold` sets the accuracy required for a match.
 
+## Available Keys and Mouse Buttons
+
+All the keys listed can be detected as well as pressed, except `xbutton1` and `xbutton2`, which cannot be pressed.
+
+### Keyboard Keys
+
+- **Alphabets**: 
+  - `a`, `A`, `b`, `B`, `c`, `C`, `d`, `D`, `e`, `E`, `f`, `F`, `g`, `G`, `h`, `H`, `i`, `I`, `j`, `J`, `k`, `K`, `l`, `L`, `m`, `M`, `n`, `N`, `o`, `O`, `p`, `P`, `q`, `Q`, `r`, `R`, `s`, `S`, `t`, `T`, `u`, `U`, `v`, `V`, `w`, `W`, `x`, `X`, `y`, `Y`, `z`, `Z`
+
+- **Numbers**: 
+  - `0`, `1`, `2`, `3`, `4`, `5`, `6`, `7`, `8`, `9`
+  - `num0`, `num1`, `num2`, `num3`, `num4`, `num5`, `num6`, `num7`, `num8`, `num9`
+
+- **Symbols**:
+  - `` ` ``, `~`, `!`, `@`, `#`, `$`, `%`, `^`, `&`, `*`, `(`, `)`, `-`, `_`, `=`, `+`, `[`, `{`, `]`, `}`, `\`, `|`, `;`, `:`, `'`, `"`, `,`, `<`, `.`, `>`, `/`, `?`
+
+- **Function Keys**: 
+  - `f1`, `f2`, `f3`, `f4`, `f5`, `f6`, `f7`, `f8`, `f9`, `f10`, `f11`, `f12`
+
+- **Control Keys**:
+  - `space`, `esc`, `tab`, `backspace`, `enter`, `numenter`, `shift`, `lshift`, `rshift`, `ctrl`, `lctrl`, `rctrl`, `alt`, `lalt`, `ralt`, `win`, `lwin`, `rwin`, `apps`, `capslock`, `numlock`, `scrolllock`, `insert`, `delete`, `home`, `end`, `pageup`, `pagedown`, `prtsc`, `sysrq`
+
+- **Arrow Keys**: 
+  - `up`, `down`, `left`, `right`
+
+### Mouse Buttons
+
+- **Primary Buttons**: 
+  - `left`, `right`, `middle`
+
+- **Additional Buttons**: 
+  - `xbutton1` (can only be detected), `xbutton2` (can only be detected)
+
 ## Example Usage
 
 ### Writing Complex Strings
 
 ```Python
 import directinput
 
 # Writing a string with special characters
-directinput.write("Hello, world!")
+directinput.write("Hello, world! ✌️")
 ```
 
 This demonstrates the enhanced write function, capable of handling a wide range of characters, surpassing limitations you might find in other modules.
 
 ### Detecting Key Presses
 
 ```Python
 import directinput
 
 # Detect if the 'A' key is being pressed
 if directinput.keyDetect('a'):
     print("The 'A' key is pressed!")
+
+# Detect if both 'left_mouse' and 'xbutton1' is being pressed
+if directinput.keyDetect(['left_mouse', 'xbutton1']):
+    print("Pressed!")
 ```
 
 ### Locating an Image on the Screen
 
 The locateImage function in WinDirectInput adds a layer of flexibility to image detection. Whether you're automating tasks based on visual cues or integrating with image processing, this function is incredibly handy.
 
 ```Python
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `WinDirectInput-1.1.0/directinput.py` & `WinDirectInput-1.2.0/directinput.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,21 +243,28 @@
 
 EXTENDED_KEYS = [
     'up', 'down', 'left', 'right', 'numenter', 'num/',
     'home', 'end', 'delete', 'insert', 'pageup', 'pagedown',
     'prtsc', 'sysrq', 'ralt', 'rctrl', 'win', 'rwin', 'lwin'
 ]
 
-# Define virtual codes for mouse input
+# Define direct codes for mouse input
 MB_CODE = {
     'left': 0x0002,
     'right': 0x0008,
     'middle': 0x0020
 }
 
+# Define virtual codes for mouse detection
+MVB_CODE = {
+    'left_mouse': 0x01,
+    'right_mouse': 0x02,
+    'middle_mouse': 0x04
+}
+
 # C struct redefinitions
 PUL = ctypes.POINTER(ctypes.c_ulong)
 
 
 class KeyBdInput(ctypes.Structure):
     _fields_ = [("wVk", ctypes.c_ushort),
                 ("wScan", ctypes.c_ushort),
@@ -806,31 +813,35 @@
     if they are currently pressed. The keys parameter can be a single key (as a string) or a list.
     The function returns True if all specified keys are pressed,
     and False if any key is not pressed or not recognized.
 
     Parameters:
     keys : str or list of str
         The key or list of keys to check. The key names should correspond to the key mappings.
+        It can take keyboard keys and also mouse buttons.
 
     Returns:
     bool
         True if all specified keys are pressed, False otherwise.
 
     Example:
     keyDetect('a')             # Check if the 'a' key is pressed.
     keyDetect(['ctrl', 'c'])   # Check if both 'ctrl' and 'c' keys are pressed.
+    keyDetect(['left_mouse'])  # Check if left mouse button is pressed.
+    keyDetect(['xbutton1'])    # Check if mouse xbutton1 is pressed.
     """
+    KEY_CODE = {**VK_CODE, **MVB_CODE}
 
     # Check if keys is a single key (string) and convert it to a list
     if isinstance(keys, str):
         keys = [keys]
 
     # Check the state of each key in the list
     for key in keys:
-        key_code = VK_CODE.get(key.lower(), None)
+        key_code = KEY_CODE.get(key.lower(), None)
         if key_code is None:
             # Handle the case where the key is not recognized
             print(f"Warning: Key '{key}' not recognized.")
             return False
 
         key_state = ctypes.windll.user32.GetAsyncKeyState(key_code)
         if key_state <= 1:
```

### Comparing `WinDirectInput-1.1.0/setup.py` & `WinDirectInput-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='WinDirectInput',
-    version='1.1.0',
+    version='1.2.0',
     author='AbdulRahim Khan',
     author_email='abdulrahimpds@gmail.com',
     description='A Windows-specific package for simulating keyboard and mouse inputs',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/abdulrahimpds/WinDirectInput',
     py_modules=['directinput'],
```

