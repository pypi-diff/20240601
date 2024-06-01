# Comparing `tmp/easy_fnc-0.1.5.tar.gz` & `tmp/easy_fnc-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_fnc-0.1.5.tar", last modified: Fri May 31 08:41:40 2024, max compression
+gzip compressed data, was "easy_fnc-0.1.6.tar", last modified: Sat Jun  1 21:13:42 2024, max compression
```

## Comparing `easy_fnc-0.1.5.tar` & `easy_fnc-0.1.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 atakantekparmak   (501) staff       (20)        0 2024-05-31 08:41:40.327350 easy_fnc-0.1.5/
--rw-r--r--   0 atakantekparmak   (501) staff       (20)    11357 2024-05-02 07:40:29.000000 easy_fnc-0.1.5/LICENSE
--rw-r--r--   0 atakantekparmak   (501) staff       (20)     5774 2024-05-31 08:41:40.327103 easy_fnc-0.1.5/PKG-INFO
--rw-r--r--   0 atakantekparmak   (501) staff       (20)     5370 2024-05-31 08:41:07.000000 easy_fnc-0.1.5/README.md
-drwxr-xr-x   0 atakantekparmak   (501) staff       (20)        0 2024-05-31 08:41:40.325507 easy_fnc-0.1.5/easy_fnc/
--rw-r--r--   0 atakantekparmak   (501) staff       (20)        0 2024-05-02 07:40:29.000000 easy_fnc-0.1.5/easy_fnc/__init__.py
--rw-r--r--   0 atakantekparmak   (501) staff       (20)      927 2024-05-04 13:37:29.000000 easy_fnc-0.1.5/easy_fnc/core_utils.py
--rw-r--r--   0 atakantekparmak   (501) staff       (20)     6818 2024-05-31 07:56:21.000000 easy_fnc-0.1.5/easy_fnc/function_caller.py
--rw-r--r--   0 atakantekparmak   (501) staff       (20)     2500 2024-05-04 14:19:47.000000 easy_fnc-0.1.5/easy_fnc/functions.py
-drwxr-xr-x   0 atakantekparmak   (501) staff       (20)        0 2024-05-31 08:41:40.326614 easy_fnc-0.1.5/easy_fnc/models/
--rw-r--r--   0 atakantekparmak   (501) staff       (20)        0 2024-05-02 07:40:29.000000 easy_fnc-0.1.5/easy_fnc/models/__init__.py
--rw-r--r--   0 atakantekparmak   (501) staff       (20)     1119 2024-05-30 12:40:49.000000 easy_fnc-0.1.5/easy_fnc/models/model.py
--rw-r--r--   0 atakantekparmak   (501) staff       (20)     4439 2024-05-30 12:39:08.000000 easy_fnc-0.1.5/easy_fnc/models/ollama.py
--rw-r--r--   0 atakantekparmak   (501) staff       (20)      233 2024-05-31 08:01:58.000000 easy_fnc-0.1.5/easy_fnc/utils.py
-drwxr-xr-x   0 atakantekparmak   (501) staff       (20)        0 2024-05-31 08:41:40.326826 easy_fnc-0.1.5/easy_fnc.egg-info/
--rw-r--r--   0 atakantekparmak   (501) staff       (20)     5774 2024-05-31 08:41:40.000000 easy_fnc-0.1.5/easy_fnc.egg-info/PKG-INFO
--rw-r--r--   0 atakantekparmak   (501) staff       (20)      376 2024-05-31 08:41:40.000000 easy_fnc-0.1.5/easy_fnc.egg-info/SOURCES.txt
--rw-r--r--   0 atakantekparmak   (501) staff       (20)        1 2024-05-31 08:41:40.000000 easy_fnc-0.1.5/easy_fnc.egg-info/dependency_links.txt
--rw-r--r--   0 atakantekparmak   (501) staff       (20)        7 2024-05-31 08:41:40.000000 easy_fnc-0.1.5/easy_fnc.egg-info/requires.txt
--rw-r--r--   0 atakantekparmak   (501) staff       (20)        9 2024-05-31 08:41:40.000000 easy_fnc-0.1.5/easy_fnc.egg-info/top_level.txt
--rw-r--r--   0 atakantekparmak   (501) staff       (20)       38 2024-05-31 08:41:40.327411 easy_fnc-0.1.5/setup.cfg
--rw-r--r--   0 atakantekparmak   (501) staff       (20)      816 2024-05-31 08:40:10.000000 easy_fnc-0.1.5/setup.py
+drwxr-xr-x   0 atakantekparmak   (501) staff       (20)        0 2024-06-01 21:13:42.399819 easy_fnc-0.1.6/
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)    11357 2024-05-02 07:40:29.000000 easy_fnc-0.1.6/LICENSE
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)     5774 2024-06-01 21:13:42.399576 easy_fnc-0.1.6/PKG-INFO
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)     5370 2024-05-31 08:41:07.000000 easy_fnc-0.1.6/README.md
+drwxr-xr-x   0 atakantekparmak   (501) staff       (20)        0 2024-06-01 21:13:42.397027 easy_fnc-0.1.6/easy_fnc/
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)        0 2024-05-02 07:40:29.000000 easy_fnc-0.1.6/easy_fnc/__init__.py
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)      927 2024-05-04 13:37:29.000000 easy_fnc-0.1.6/easy_fnc/core_utils.py
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)     8014 2024-06-01 21:12:32.000000 easy_fnc-0.1.6/easy_fnc/function_caller.py
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)     2500 2024-05-04 14:19:47.000000 easy_fnc-0.1.6/easy_fnc/functions.py
+drwxr-xr-x   0 atakantekparmak   (501) staff       (20)        0 2024-06-01 21:13:42.398458 easy_fnc-0.1.6/easy_fnc/models/
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)        0 2024-05-02 07:40:29.000000 easy_fnc-0.1.6/easy_fnc/models/__init__.py
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)     1119 2024-05-30 12:40:49.000000 easy_fnc-0.1.6/easy_fnc/models/model.py
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)     4439 2024-05-30 12:39:08.000000 easy_fnc-0.1.6/easy_fnc/models/ollama.py
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)      233 2024-05-31 08:01:58.000000 easy_fnc-0.1.6/easy_fnc/utils.py
+drwxr-xr-x   0 atakantekparmak   (501) staff       (20)        0 2024-06-01 21:13:42.398991 easy_fnc-0.1.6/easy_fnc.egg-info/
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)     5774 2024-06-01 21:13:42.000000 easy_fnc-0.1.6/easy_fnc.egg-info/PKG-INFO
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)      376 2024-06-01 21:13:42.000000 easy_fnc-0.1.6/easy_fnc.egg-info/SOURCES.txt
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)        1 2024-06-01 21:13:42.000000 easy_fnc-0.1.6/easy_fnc.egg-info/dependency_links.txt
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)        7 2024-06-01 21:13:42.000000 easy_fnc-0.1.6/easy_fnc.egg-info/requires.txt
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)        9 2024-06-01 21:13:42.000000 easy_fnc-0.1.6/easy_fnc.egg-info/top_level.txt
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)       38 2024-06-01 21:13:42.399880 easy_fnc-0.1.6/setup.cfg
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)      816 2024-06-01 21:13:40.000000 easy_fnc-0.1.6/setup.py
```

### Comparing `easy_fnc-0.1.5/LICENSE` & `easy_fnc-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_fnc-0.1.5/PKG-INFO` & `easy_fnc-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy_fnc
-Version: 0.1.5
+Version: 0.1.6
 Summary: This package hopes to provide a modular and highly extendable interface to interact with LLMs via (multiple) function calling, easily.
 Home-page: https://github.com/AtakanTekparmak/easy_fnc
 Author: Atakan Tekparmak
 Author-email: atakantekerparmak@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ollama
```

### Comparing `easy_fnc-0.1.5/README.md` & `easy_fnc-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `easy_fnc-0.1.5/easy_fnc/core_utils.py` & `easy_fnc-0.1.6/easy_fnc/core_utils.py`

 * *Files identical despite different names*

### Comparing `easy_fnc-0.1.5/easy_fnc/function_caller.py` & `easy_fnc-0.1.6/easy_fnc/function_caller.py`

 * *Files 18% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     
         def check_if_input_is_output(input: dict) -> dict:
             """Check if the input is an output from a previous function."""
             for key, value in input.items():
                 if value in self.outputs:
                     input[key] = self.outputs[value]
                 # Check if value is a string encased by dollar signs
-                if value.startswith("$") and value.endswith("$"):
+                if value.startswith("$") and value.endswith("$") and not key.lower() == "key":
                     input[key] = self.outputs[value[1:-1]]
             return input
         
         def check_if_input_is_function(input: dict) -> dict:
             """Check if the input is a function."""
             # Currently experimental, not working as expected
             for key, value in input.items():
@@ -90,14 +90,20 @@
             return input
         
         def format_input(input: dict) -> dict:
             """Format the input for the function."""
             for key, value in input.items():
                 if not isinstance(value, str):
                     input[key] = str(value)
+                    if input[key].startswith("$") and input[key].endswith("$") and not key.lower() == "key":
+                        input[key] = input[key][1:-1]
+                        if input[key] in self.outputs:
+                            input[key] = self.outputs[value]
+                if isinstance(value, int):
+                    input[key] = value
                 # If a value is encased by "{" and "}", then it is a variable
                 if "{" in value and "}" in value:
                     # Get the variable name
                     variable_name = value.split("{")[1].split("}")[0]
                     # Get the value from the outputs
                     input[key] = variable_name 
             
@@ -107,38 +113,52 @@
             """Infer the input type for the function."""
             for key, value in input.items():
                 # If the value is a string, then check if it is a number
                 if isinstance(value, str):
                     # Check if the value is an integer
                     if value.isdigit():
                         input[key] = int(value)
+                    elif value.startswith("$") and value.endswith("$") and not key.lower() == "key":
+                        input[key] = self.outputs[value[1:-1]]
                     # Check if the value is a float
                     elif "." in value and value.replace(".", "").isdigit():
                         input[key] = float(value)
                     # Check if the value is a boolean
                     elif value.lower() in ["true", "false"]:
                         input[key] = value.lower() == "true"
                     # Check if the value is a list
                     elif value.startswith("[") and value.endswith("]"):
                         input[key] = literal_eval(value)
                     # Check if the value is a dictionary
                     elif value.startswith("{") and value.endswith("}"):
                         input[key] = literal_eval(value)
             
             return input
+        
+        def remove_the_dollarsign(input: dict) -> dict:
+            """Removes the dollarsign from the input."""
+            for key, value in input.items():
+                if isinstance(value, str):
+                    if value.startswith("$") and value.endswith("$") and not key.lower() == "key":
+                        input[key] = value[1:-1]
+                        input[key] = self.outputs[input[key]]
+                if isinstance(value, dict):
+                    input[key] = remove_the_dollarsign(value)
+            return input
 
         # Get the function name from the function dictionary
         function_name = function["name"]
         
         # Get the function params from the function dictionary
         function_input = function["params"] if "params" in function else None
         function_input = format_input(function_input) if function_input else None
         function_input = check_if_input_is_output(function_input) if function_input else None
         function_input = check_if_input_is_function(function_input) if function_input else None
         function_input = infer_input_type(function_input) if function_input else None
+        function_input = remove_the_dollarsign(function_input) if function_input else None
     
         # Call the function from tools.py with the given input
         # pass all the arguments to the function from the function_input
         output = self.functions[function_name](**function_input) if function_input else self.functions[function_name]()
         # Check if output is enclosed by dollar signs
         if isinstance(output, str):
             if output.startswith("$") and output.endswith("$"):
```

### Comparing `easy_fnc-0.1.5/easy_fnc/functions.py` & `easy_fnc-0.1.6/easy_fnc/functions.py`

 * *Files identical despite different names*

### Comparing `easy_fnc-0.1.5/easy_fnc/models/model.py` & `easy_fnc-0.1.6/easy_fnc/models/model.py`

 * *Files identical despite different names*

### Comparing `easy_fnc-0.1.5/easy_fnc/models/ollama.py` & `easy_fnc-0.1.6/easy_fnc/models/ollama.py`

 * *Files identical despite different names*

### Comparing `easy_fnc-0.1.5/easy_fnc.egg-info/PKG-INFO` & `easy_fnc-0.1.6/easy_fnc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy_fnc
-Version: 0.1.5
+Version: 0.1.6
 Summary: This package hopes to provide a modular and highly extendable interface to interact with LLMs via (multiple) function calling, easily.
 Home-page: https://github.com/AtakanTekparmak/easy_fnc
 Author: Atakan Tekparmak
 Author-email: atakantekerparmak@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ollama
```

### Comparing `easy_fnc-0.1.5/setup.py` & `easy_fnc-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     """Read the README.md file and return its contents."""
     with open("README.md", "r", encoding="utf-8") as fh:
         return fh.read()
 
 def main():
     setup(
         name='easy_fnc',
-        version='0.1.5',
+        version='0.1.6',
         description='This package hopes to provide a modular and highly extendable interface to interact with LLMs via (multiple) function calling, easily.',
         long_description=read_readme(),
         long_description_content_type="text/markdown",
         author='Atakan Tekparmak',
         author_email='atakantekerparmak@gmail.com',
         url="https://github.com/AtakanTekparmak/easy_fnc",
         packages=find_packages(),
```

