# Comparing `tmp/subspy-2.2.2.tar.gz` & `tmp/subspy-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subspy-2.2.2.tar", last modified: Sat Jun  1 05:55:03 2024, max compression
+gzip compressed data, was "subspy-2.2.3.tar", last modified: Sat Jun  1 07:16:24 2024, max compression
```

## Comparing `subspy-2.2.2.tar` & `subspy-2.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 05:55:03.772989 subspy-2.2.2/
--rw-rw-rw-   0        0        0     2426 2024-06-01 05:55:03.772989 subspy-2.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1687 2024-06-01 05:54:51.000000 subspy-2.2.2/README.md
--rw-rw-rw-   0        0        0       42 2024-06-01 05:55:03.772989 subspy-2.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1252 2024-06-01 05:54:51.000000 subspy-2.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-06-01 05:55:03.741755 subspy-2.2.2/subspy/
--rw-rw-rw-   0        0        0      258 2024-06-01 05:54:51.000000 subspy-2.2.2/subspy/__init__.py
--rw-rw-rw-   0        0        0     2176 2024-06-01 05:54:51.000000 subspy-2.2.2/subspy/cli.py
--rw-rw-rw-   0        0        0    72949 2024-06-01 05:54:51.000000 subspy-2.2.2/subspy/default_subdomains.txt
--rw-rw-rw-   0        0        0     1458 2024-06-01 05:54:51.000000 subspy-2.2.2/subspy/subdomain.py
-drwxrwxrwx   0        0        0        0 2024-06-01 05:55:03.772989 subspy-2.2.2/subspy.egg-info/
--rw-rw-rw-   0        0        0     2426 2024-06-01 05:55:03.000000 subspy-2.2.2/subspy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2024-06-01 05:55:03.000000 subspy-2.2.2/subspy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 05:55:03.000000 subspy-2.2.2/subspy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-06-01 05:55:03.000000 subspy-2.2.2/subspy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2024-06-01 05:55:03.000000 subspy-2.2.2/subspy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-06-01 05:55:03.000000 subspy-2.2.2/subspy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 07:16:24.019671 subspy-2.2.3/
+-rw-rw-rw-   0        0        0     2914 2024-06-01 07:16:24.019671 subspy-2.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2156 2024-06-01 07:14:35.000000 subspy-2.2.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-06-01 07:16:24.019671 subspy-2.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1252 2024-06-01 07:14:35.000000 subspy-2.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 07:16:23.952677 subspy-2.2.3/subspy/
+-rw-rw-rw-   0        0        0      258 2024-06-01 07:14:35.000000 subspy-2.2.3/subspy/__init__.py
+-rw-rw-rw-   0        0        0     4294 2024-06-01 07:14:35.000000 subspy-2.2.3/subspy/cli.py
+-rw-rw-rw-   0        0        0    72949 2024-06-01 07:14:35.000000 subspy-2.2.3/subspy/default_subdomains.txt
+-rw-rw-rw-   0        0        0     1602 2024-06-01 07:14:35.000000 subspy-2.2.3/subspy/subdomain.py
+drwxrwxrwx   0        0        0        0 2024-06-01 07:16:24.017487 subspy-2.2.3/subspy.egg-info/
+-rw-rw-rw-   0        0        0     2914 2024-06-01 07:16:23.000000 subspy-2.2.3/subspy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2024-06-01 07:16:23.000000 subspy-2.2.3/subspy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 07:16:23.000000 subspy-2.2.3/subspy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-06-01 07:16:23.000000 subspy-2.2.3/subspy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2024-06-01 07:16:23.000000 subspy-2.2.3/subspy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-06-01 07:16:23.000000 subspy-2.2.3/subspy.egg-info/top_level.txt
```

### Comparing `subspy-2.2.2/PKG-INFO` & `subspy-2.2.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subspy
-Version: 2.2.2
+Version: 2.2.3
 Summary: SubSpy: A tool for subdomain enumeration.
 Home-page: https://mrfidal.in/cyber-security/subspy
 Author: Fidal
 Author-email: mrfidal@proton.me
 License: MIT
 Keywords: subspy,subdomain,enumeration,scanning,mrfidal,cyber security
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,52 +17,71 @@
 Description-Content-Type: text/markdown
 
 # Subspy
 
 Subspy is a powerful subdomain enumeration tool designed to help you discover subdomains for a given base URL. It provides a comprehensive set of features and options to enhance your subdomain reconnaissance process.
 
 ## Benefits
-- **Efficiency** : Quickly identify potential attack surfaces and gather information about a target's infrastructure.
-- **Flexibility** : Customize subdomain tests using custom subdomain lists or default lists included in the tool.
-- **Ease of Use** : Simple command-line interface with clear options and informative output.
-- **Versatility** : Save results to files for further analysis or reporting.
+- **Efficiency**: Quickly identify potential attack surfaces and gather information about a target's infrastructure.
+- **Flexibility**: Customize subdomain tests using custom subdomain lists or default lists included in the tool.
+- **Ease of Use**: Simple command-line interface with clear options and informative output.
+- **Versatility**: Save results to files for further analysis or reporting.
 
 ## Installation
 
 Install Subspy using pip:
 
 ```bash
 pip install subspy
 ```
+
 ## Usage
 
 ```bash
 subspy --url https://example.com
 ```
+
 ### Command Line Options
 - **--url** : The base URL to test subdomains against (e.g., https://example.com).
 - **--sub-list** : The file containing a list of subdomains to test.
 - **--save** : Save the output to a file.
 - **--version** : Show the version of the tool.
+- **--silent** : Suppress output of wrong subdomains, only print found subdomains.
+- **--time** : Run the tool for a specific amount of time (e.g., 5m, 50s, 1h).
 
 ### Examples
 - Test subdomains for a specific URL:
 ```bash
 subspy --url https://example.com
 ```
 - Specify a custom subdomain list file:
 ```bash
 subspy --url https://example.com --sub-list subdomains.txt
 ```
 - Save the output to a file:
-```bash
+```
 subspy --url https://example.com --save output.txt
+````
+- Run in silent mode (only print found subdomains):
+```bash
+subspy --url https://example.com --silent
+````
+- Run the tool for a specific amount of time:
+```bash
+subspy --url https://example.com --time 5m
+```
+- Combine silent mode and time limit:
+```bash
+subspy --url https://example.com --silent --time 1h
 ```
 - Show the version of the tool:
 ```bash
 subspy --version
 ```
+
 ### Disclaimer
 
 This tool is provided for educational and informational purposes only. The author and contributors of Subspy are not responsible for any misuse or illegal activities performed using this tool.
-#### Thanks
+
+### Thanks
+
 Thank you ❤ for using Subspy and supporting open-source tools!
```

### Comparing `subspy-2.2.2/README.md` & `subspy-2.2.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,69 @@
 # Subspy
 
 Subspy is a powerful subdomain enumeration tool designed to help you discover subdomains for a given base URL. It provides a comprehensive set of features and options to enhance your subdomain reconnaissance process.
 
 ## Benefits
-- **Efficiency** : Quickly identify potential attack surfaces and gather information about a target's infrastructure.
-- **Flexibility** : Customize subdomain tests using custom subdomain lists or default lists included in the tool.
-- **Ease of Use** : Simple command-line interface with clear options and informative output.
-- **Versatility** : Save results to files for further analysis or reporting.
+- **Efficiency**: Quickly identify potential attack surfaces and gather information about a target's infrastructure.
+- **Flexibility**: Customize subdomain tests using custom subdomain lists or default lists included in the tool.
+- **Ease of Use**: Simple command-line interface with clear options and informative output.
+- **Versatility**: Save results to files for further analysis or reporting.
 
 ## Installation
 
 Install Subspy using pip:
 
 ```bash
 pip install subspy
 ```
+
 ## Usage
 
 ```bash
 subspy --url https://example.com
 ```
+
 ### Command Line Options
 - **--url** : The base URL to test subdomains against (e.g., https://example.com).
 - **--sub-list** : The file containing a list of subdomains to test.
 - **--save** : Save the output to a file.
 - **--version** : Show the version of the tool.
+- **--silent** : Suppress output of wrong subdomains, only print found subdomains.
+- **--time** : Run the tool for a specific amount of time (e.g., 5m, 50s, 1h).
 
 ### Examples
 - Test subdomains for a specific URL:
 ```bash
 subspy --url https://example.com
 ```
 - Specify a custom subdomain list file:
 ```bash
 subspy --url https://example.com --sub-list subdomains.txt
 ```
 - Save the output to a file:
-```bash
+```
 subspy --url https://example.com --save output.txt
+````
+- Run in silent mode (only print found subdomains):
+```bash
+subspy --url https://example.com --silent
+````
+- Run the tool for a specific amount of time:
+```bash
+subspy --url https://example.com --time 5m
+```
+- Combine silent mode and time limit:
+```bash
+subspy --url https://example.com --silent --time 1h
 ```
 - Show the version of the tool:
 ```bash
 subspy --version
 ```
+
 ### Disclaimer
 
 This tool is provided for educational and informational purposes only. The author and contributors of Subspy are not responsible for any misuse or illegal activities performed using this tool.
-#### Thanks
+
+### Thanks
+
 Thank you ❤ for using Subspy and supporting open-source tools!
```

### Comparing `subspy-2.2.2/setup.py` & `subspy-2.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as readme_file:
     long_description = readme_file.read()
 
 setup(
     name='subspy',
-    version='2.2.2',
+    version='2.2.3',
     description='SubSpy: A tool for subdomain enumeration.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://mrfidal.in/cyber-security/subspy',
     author='Fidal',
     author_email='mrfidal@proton.me',
     license='MIT',
```

### Comparing `subspy-2.2.2/subspy/default_subdomains.txt` & `subspy-2.2.3/subspy/default_subdomains.txt`

 * *Files identical despite different names*

### Comparing `subspy-2.2.2/subspy/subdomain.py` & `subspy-2.2.3/subspy/subdomain.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,27 +12,31 @@
 def fix_url(url):
     if url.startswith("http://"):
         return url[len("http://"):]
     elif url.startswith("https://"):
         return url[len("https://"):]
     return url
 
-def test_subdomains(url, subdomains):
-    tried_subdomains = []
+def test_subdomains(url, subdomains, silent, stop_event, tried_count, found_count):
     found_subdomains = []
     fixed_url = fix_url(url)
     for idx, subdomain in enumerate(subdomains, start=1):
+        if stop_event.is_set():
+            break
         url_with_subdomain = f"https://{subdomain}.{fixed_url}"
-        tried_subdomains.append(url_with_subdomain)
+        tried_count[0] += 1
         available, status_code = is_subdomain_available(url_with_subdomain)
         if available:
             found_subdomains.append(subdomain)
-            print(f" ({idx}/{len(subdomains)}) Subdomain found : {subdomain}.{fixed_url} Status Code : {status_code}")
+            found_count[0] += 1
+            if not silent:
+                print(f" ({idx}/{len(subdomains)}) Subdomain found : {subdomain}.{fixed_url} Status Code : {status_code}")
         else:
-            print(f" ({idx}/{len(subdomains)}) Wrong Subdomain : {subdomain}.{fixed_url} Status Code : {status_code}")
+            if not silent:
+                print(f" ({idx}/{len(subdomains)}) Wrong Subdomain : {subdomain}.{fixed_url} Status Code : {status_code}")
 
     return found_subdomains
 
 def get_default_subdomains():
     current_dir = os.path.dirname(__file__)
     default_subdomains_path = os.path.join(current_dir, "default_subdomains.txt")
     with open(default_subdomains_path, "r") as file:
```

### Comparing `subspy-2.2.2/subspy.egg-info/PKG-INFO` & `subspy-2.2.3/subspy.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subspy
-Version: 2.2.2
+Version: 2.2.3
 Summary: SubSpy: A tool for subdomain enumeration.
 Home-page: https://mrfidal.in/cyber-security/subspy
 Author: Fidal
 Author-email: mrfidal@proton.me
 License: MIT
 Keywords: subspy,subdomain,enumeration,scanning,mrfidal,cyber security
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,52 +17,71 @@
 Description-Content-Type: text/markdown
 
 # Subspy
 
 Subspy is a powerful subdomain enumeration tool designed to help you discover subdomains for a given base URL. It provides a comprehensive set of features and options to enhance your subdomain reconnaissance process.
 
 ## Benefits
-- **Efficiency** : Quickly identify potential attack surfaces and gather information about a target's infrastructure.
-- **Flexibility** : Customize subdomain tests using custom subdomain lists or default lists included in the tool.
-- **Ease of Use** : Simple command-line interface with clear options and informative output.
-- **Versatility** : Save results to files for further analysis or reporting.
+- **Efficiency**: Quickly identify potential attack surfaces and gather information about a target's infrastructure.
+- **Flexibility**: Customize subdomain tests using custom subdomain lists or default lists included in the tool.
+- **Ease of Use**: Simple command-line interface with clear options and informative output.
+- **Versatility**: Save results to files for further analysis or reporting.
 
 ## Installation
 
 Install Subspy using pip:
 
 ```bash
 pip install subspy
 ```
+
 ## Usage
 
 ```bash
 subspy --url https://example.com
 ```
+
 ### Command Line Options
 - **--url** : The base URL to test subdomains against (e.g., https://example.com).
 - **--sub-list** : The file containing a list of subdomains to test.
 - **--save** : Save the output to a file.
 - **--version** : Show the version of the tool.
+- **--silent** : Suppress output of wrong subdomains, only print found subdomains.
+- **--time** : Run the tool for a specific amount of time (e.g., 5m, 50s, 1h).
 
 ### Examples
 - Test subdomains for a specific URL:
 ```bash
 subspy --url https://example.com
 ```
 - Specify a custom subdomain list file:
 ```bash
 subspy --url https://example.com --sub-list subdomains.txt
 ```
 - Save the output to a file:
-```bash
+```
 subspy --url https://example.com --save output.txt
+````
+- Run in silent mode (only print found subdomains):
+```bash
+subspy --url https://example.com --silent
+````
+- Run the tool for a specific amount of time:
+```bash
+subspy --url https://example.com --time 5m
+```
+- Combine silent mode and time limit:
+```bash
+subspy --url https://example.com --silent --time 1h
 ```
 - Show the version of the tool:
 ```bash
 subspy --version
 ```
+
 ### Disclaimer
 
 This tool is provided for educational and informational purposes only. The author and contributors of Subspy are not responsible for any misuse or illegal activities performed using this tool.
-#### Thanks
+
+### Thanks
+
 Thank you ❤ for using Subspy and supporting open-source tools!
```

