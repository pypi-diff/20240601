# Comparing `tmp/llama3_package-0.3.0.tar.gz` & `tmp/llama3_package-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama3_package-0.3.0.tar", last modified: Mon May 20 14:01:37 2024, max compression
+gzip compressed data, was "llama3_package-0.5.0.tar", last modified: Sat Jun  1 10:39:12 2024, max compression
```

## Comparing `llama3_package-0.3.0.tar` & `llama3_package-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:01:37.576204 llama3_package-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-05-20 14:01:37.576204 llama3_package-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-20 14:01:24.000000 llama3_package-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-20 14:01:24.000000 llama3_package-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 14:01:37.576204 llama3_package-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-20 14:01:24.000000 llama3_package-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:01:37.576204 llama3_package-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:01:37.576204 llama3_package-0.3.0/src/llama3/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-20 14:01:24.000000 llama3_package-0.3.0/src/llama3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-20 14:01:24.000000 llama3_package-0.3.0/src/llama3/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5431 2024-05-20 14:01:24.000000 llama3_package-0.3.0/src/llama3/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-20 14:01:24.000000 llama3_package-0.3.0/src/llama3/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:01:37.576204 llama3_package-0.3.0/src/llama3_package.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-05-20 14:01:37.000000 llama3_package-0.3.0/src/llama3_package.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-20 14:01:37.000000 llama3_package-0.3.0/src/llama3_package.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 14:01:37.000000 llama3_package-0.3.0/src/llama3_package.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-20 14:01:37.000000 llama3_package-0.3.0/src/llama3_package.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 14:01:37.000000 llama3_package-0.3.0/src/llama3_package.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:39:12.447529 llama3_package-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-06-01 10:39:12.447529 llama3_package-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-06-01 10:39:03.000000 llama3_package-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-06-01 10:39:03.000000 llama3_package-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 10:39:12.447529 llama3_package-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-06-01 10:39:03.000000 llama3_package-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:39:12.443529 llama3_package-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:39:12.443529 llama3_package-0.5.0/src/llama3/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-06-01 10:39:03.000000 llama3_package-0.5.0/src/llama3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-06-01 10:39:03.000000 llama3_package-0.5.0/src/llama3/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-06-01 10:39:03.000000 llama3_package-0.5.0/src/llama3/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-06-01 10:39:03.000000 llama3_package-0.5.0/src/llama3/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:39:12.447529 llama3_package-0.5.0/src/llama3_package.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-06-01 10:39:12.000000 llama3_package-0.5.0/src/llama3_package.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-06-01 10:39:12.000000 llama3_package-0.5.0/src/llama3_package.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 10:39:12.000000 llama3_package-0.5.0/src/llama3_package.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-06-01 10:39:12.000000 llama3_package-0.5.0/src/llama3_package.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-06-01 10:39:12.000000 llama3_package-0.5.0/src/llama3_package.egg-info/top_level.txt
```

### Comparing `llama3_package-0.3.0/PKG-INFO` & `llama3_package-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama3_package
-Version: 0.3.0
+Version: 0.5.0
 Summary: A Python package to interact with Llama 3 locally using Ollama.
 Home-page: https://github.com/princeDisant/llama3_package
 Author: Disant Upadhyay
 License: UNKNOWN
 Description: # Llama3 Package
         
         ## Overview
```

### Comparing `llama3_package-0.3.0/README.md` & `llama3_package-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `llama3_package-0.3.0/pyproject.toml` & `llama3_package-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `llama3_package-0.3.0/setup.py` & `llama3_package-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="llama3_package",
-    version="0.3.0",
+    version="0.5.0",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     install_requires=[
         "langchain",
         "notebook",
         "ollama",
     ],
```

### Comparing `llama3_package-0.3.0/src/llama3/model.py` & `llama3_package-0.5.0/src/llama3/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 class Llama3Model:
     def __init__(self):
         self.model_name = Config.MODEL_NAME
         self.ollama_server_process = None
         self.ollama_process = None
         self._install_ollama()
         self._start_ollama_server()
-        self._ensure_server_is_running()
+#         self._ensure_server_is_running()
         self._pull_model()
         self._start_ollama()
         logger.info(f"Initialized Llama3 model with model name: {self.model_name}")
         atexit.register(self._stop_ollama)
 
     def _install_ollama(self):
         system = platform.system()
@@ -51,15 +51,15 @@
         except subprocess.CalledProcessError as e:
             logger.error(f"Error starting Ollama server: {e.stderr}")
             raise
 
     def _ensure_server_is_running(self, retries=5, delay=5):
         for attempt in range(retries):
             try:
-                response = requests.get("http://127.0.0.1:11434/api/version")
+                response = requests.get("http://127.0.0.1:11434")
                 if response.status_code == 200:
                     logger.info("Ollama server is running.")
                     return True
             except requests.ConnectionError:
                 logger.warning(f"Attempt {attempt + 1}/{retries}: Ollama server is not running yet. Retrying in {delay} seconds...")
                 time.sleep(delay)
         raise RuntimeError("Ollama server did not start successfully.")
@@ -95,43 +95,42 @@
             logger.info("Ollama stopped.")
         if self.ollama_server_process:
             logger.info("Stopping Ollama server...")
             self.ollama_server_process.terminate()
             self.ollama_server_process.wait()
             logger.info("Ollama server stopped.")
 
+    def _run_ollama(self):
+        try:
+            logger.info(f"Running Ollama with model {self.model_name}...")
+            self.ollama_process = subprocess.Popen([
+                "docker", "exec", "-i", self.ollama_container_name,
+                "ollama", "run", self.model_name
+            ], stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
+            logger.info(f"Ollama is running with model {self.model_name}.")
+        except subprocess.CalledProcessError as e:
+            logger.error(f"Error running Ollama: {e}")
+            raise
+
     def prompt(self, text):
         try:
             logger.info(f"Sending prompt: {text}")
-            process = subprocess.run(["ollama", "run", self.model_name], input=text, text=True, capture_output=True, check=True)
+            self.ollama_process.stdin.write(text + '\n')
+            self.ollama_process.stdin.flush()
+            response = self.ollama_process.stdout.readline().strip()
             logger.info(f"Prompt successful: {text}")
-            return process.stdout
-        except subprocess.CalledProcessError as e:
-            logger.error(f"Error in prompt: {e.stderr}")
+            return response
+        except Exception as e:
+            logger.error(f"Error in prompt: {e}")
             raise
 
     def stream_prompt(self, text):
         try:
             logger.info(f"Starting streaming prompt: {text}")
-            process = subprocess.Popen(
-                ["ollama", "run", self.model_name],
-                stdin=subprocess.PIPE,
-                stdout=subprocess.PIPE,
-                stderr=subprocess.PIPE,
-                text=True
-            )
-            process.stdin.write(text)
-            process.stdin.close()
-            for line in process.stdout:
+            self.ollama_process.stdin.write(text + '\n')
+            self.ollama_process.stdin.flush()
+            for line in self.ollama_process.stdout:
                 yield line.strip()
             logger.info(f"Streaming prompt successful: {text}")
-            process.wait()
-            if process.returncode != 0:
-                raise subprocess.CalledProcessError(
-                    returncode=process.returncode,
-                    cmd=process.args,
-                    output=process.stdout.read(),
-                    stderr=process.stderr.read()
-                )
-        except subprocess.CalledProcessError as e:
-            logger.error(f"Error in stream_prompt: {e.stderr}")
-            raise
+        except Exception as e:
+            logger.error(f"Error in stream_prompt: {e}")
+            raise
```

### Comparing `llama3_package-0.3.0/src/llama3_package.egg-info/PKG-INFO` & `llama3_package-0.5.0/src/llama3_package.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama3-package
-Version: 0.3.0
+Version: 0.5.0
 Summary: A Python package to interact with Llama 3 locally using Ollama.
 Home-page: https://github.com/princeDisant/llama3_package
 Author: Disant Upadhyay
 License: UNKNOWN
 Description: # Llama3 Package
         
         ## Overview
```

