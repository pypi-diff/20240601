# Comparing `tmp/openai_voicestream-0.1.0.tar.gz` & `tmp/openai_voicestream-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_voicestream-0.1.0.tar", last modified: Sat Jun  1 17:52:53 2024, max compression
+gzip compressed data, was "openai_voicestream-0.1.1.tar", last modified: Sat Jun  1 18:00:53 2024, max compression
```

## Comparing `openai_voicestream-0.1.0.tar` & `openai_voicestream-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:52:53.677289 openai_voicestream-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     6836 2024-06-01 17:52:53.677289 openai_voicestream-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-06-01 17:52:49.000000 openai_voicestream-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:52:53.677289 openai_voicestream-0.1.0/Voice_generator/
--rw-r--r--   0 runner    (1001) docker     (127)     9849 2024-06-01 17:52:49.000000 openai_voicestream-0.1.0/Voice_generator/VoiceProcessor.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:52:49.000000 openai_voicestream-0.1.0/Voice_generator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:52:53.677289 openai_voicestream-0.1.0/openai_voicestream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6836 2024-06-01 17:52:53.000000 openai_voicestream-0.1.0/openai_voicestream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-06-01 17:52:53.000000 openai_voicestream-0.1.0/openai_voicestream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 17:52:53.000000 openai_voicestream-0.1.0/openai_voicestream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-01 17:52:53.000000 openai_voicestream-0.1.0/openai_voicestream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-01 17:52:53.000000 openai_voicestream-0.1.0/openai_voicestream.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 17:52:53.677289 openai_voicestream-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-06-01 17:52:49.000000 openai_voicestream-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 18:00:53.412897 openai_voicestream-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     6612 2024-06-01 18:00:53.412897 openai_voicestream-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-06-01 18:00:49.000000 openai_voicestream-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 18:00:53.412897 openai_voicestream-0.1.1/Voice_generator/
+-rw-r--r--   0 runner    (1001) docker     (127)     9850 2024-06-01 18:00:49.000000 openai_voicestream-0.1.1/Voice_generator/VoiceProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 18:00:49.000000 openai_voicestream-0.1.1/Voice_generator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 18:00:53.412897 openai_voicestream-0.1.1/openai_voicestream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6612 2024-06-01 18:00:53.000000 openai_voicestream-0.1.1/openai_voicestream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-06-01 18:00:53.000000 openai_voicestream-0.1.1/openai_voicestream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 18:00:53.000000 openai_voicestream-0.1.1/openai_voicestream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-06-01 18:00:53.000000 openai_voicestream-0.1.1/openai_voicestream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-01 18:00:53.000000 openai_voicestream-0.1.1/openai_voicestream.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 18:00:53.412897 openai_voicestream-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-06-01 18:00:49.000000 openai_voicestream-0.1.1/setup.py
```

### Comparing `openai_voicestream-0.1.0/PKG-INFO` & `openai_voicestream-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 Metadata-Version: 2.1
 Name: openai_voicestream
-Version: 0.1.0
+Version: 0.1.1
 Summary: A library for real-time text to speech processing using OpenAI API.
 Home-page: https://github.com/kristofferv98/openai-voicestream.git
 Author: Kristoffer Vatnehol
 Author-email: kristoffer.vatnehol@gmail.com
 License: MIT
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: pyaudio
 Requires-Dist: httpx
+Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: flake8; extra == "dev"
 
 # OpenAI VoiceStream
 
 OpenAI VoiceStream is a Python library that provides real-time text-to-speech functionality using the OpenAI API. It allows you to process text and token streams and generate audio output on-the-fly, making it suitable for integration with language models that generate responses in segments.
 
 ## Features
```

### Comparing `openai_voicestream-0.1.0/README.md` & `openai_voicestream-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `openai_voicestream-0.1.0/Voice_generator/VoiceProcessor.py` & `openai_voicestream-0.1.1/Voice_generator/VoiceProcessor.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import pyaudio
 import httpx
 import logging
 from queue import Queue, Empty
 
 # Setup logging
-logging.basicConfig(level=logging.DEBUG, format='%(asctime)s - %(levelname)s - %(message)s')
+#logging.basicConfig(level=logging.DEBUG, format='%(asctime)s - %(levelname)s - %(message)s')
 
 
 class VoiceProcessor:
     """
     A class to process and generate audio from text using the OpenAI API.
 
     Attributes:
```

### Comparing `openai_voicestream-0.1.0/openai_voicestream.egg-info/PKG-INFO` & `openai_voicestream-0.1.1/openai_voicestream.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 Metadata-Version: 2.1
 Name: openai_voicestream
-Version: 0.1.0
+Version: 0.1.1
 Summary: A library for real-time text to speech processing using OpenAI API.
 Home-page: https://github.com/kristofferv98/openai-voicestream.git
 Author: Kristoffer Vatnehol
 Author-email: kristoffer.vatnehol@gmail.com
 License: MIT
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: pyaudio
 Requires-Dist: httpx
+Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: flake8; extra == "dev"
 
 # OpenAI VoiceStream
 
 OpenAI VoiceStream is a Python library that provides real-time text-to-speech functionality using the OpenAI API. It allows you to process text and token streams and generate audio output on-the-fly, making it suitable for integration with language models that generate responses in segments.
 
 ## Features
```

### Comparing `openai_voicestream-0.1.0/setup.py` & `openai_voicestream-0.1.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from setuptools import setup, find_packages
 
 setup(
     name='openai_voicestream',
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(),
     include_package_data=True,
     license='MIT',
     description='A library for real-time text to speech processing using OpenAI API.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=[
         'pyaudio',
         'httpx',
     ],
-    url='https://github.com/kristofferv98/openai-voicestream.git',
+    extras_require={
+        'dev': [
+            'pytest',
+            'flake8'
+        ]
+    },
     author='Kristoffer Vatnehol',
     author_email='kristoffer.vatnehol@gmail.com',
+    python_requires='>=3.6',
+    url='https://github.com/kristofferv98/openai-voicestream.git',
     classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
+        'License :: OSI Approved :: MIT License',
+        'Operating System :: OS Independent',
     ],
 )
```

